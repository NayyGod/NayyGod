local ds = game:GetService("DataStoreService"):GetDataStore("Whitelist")
local bl = { -- Blacklisted Players
"xlRosita",
}


game.Players.PlayerAdded:Connect(function(plr)
local check = function()
for i,v in pairs(bl) do
if v == plr.Name then
plr:Kick("bye bye kid")
return "Blacklisted";
else
return "wl"
end
end
end
if check() == "wl" then
if not ds:GetAsync(plr.Name) == "true1" then
ds:SetAsync(plr.Name, "true1")
print("Player " ..plr.Name.. " was just whitelisted!")
else
print("Whitelisted Player Joined!")
end
end
check()
end)
