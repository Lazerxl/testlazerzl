if Key == "KEY1"
  or Key == "KEY2"
    or Key == "KEY3" then
if DiscordId == "DiscordId1"
  or DiscordId == "DiscordId2"
    or DiscordId == "DiscordId3" then
local HWID = {
   "HWID1",
   "HWID2",
   "HWID3"
}

local Old = game:GetService("RbxAnalyticsService"):GetClientId()

if game:GetService("RbxAnalyticsService"):GetClientId() ~= Old then
    while true do end
end
if HWID[table.find(HWID, Old)] == Old then
print("Whitelist")
--scripthub
else
    setclipboard("HWID : "..tostring(Old))
    game.Players.LocalPlayer:Kick("Hwid Copy!")
    wait(.5)
    game:Shutdown()
end
else
    game.Player.LocalPlayer:kick("Not Found Keys")
end
else
    game.Player.LocalPlayer:kick("Not Found DiscordId")
end
