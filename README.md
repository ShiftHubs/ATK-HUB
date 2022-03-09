--Dark Dex
spawn(function()
    while wait() do
        pcall(function()
            for i,v in pairs(game:GetService("CoreGui"):GetDescendants()) do 
                if v.Name == "ExplorerPanel" then
                    game.Players.LocalPlayer:Kick("Dark")
                end
            end
        end)
    end
end)


local HWID = {
   "HWID",
   "HWID",
   "HWID",
   "HWID"
}

local Old = game:GetService("RbxAnalyticsService"):GetClientId()

if game:GetService("RbxAnalyticsService"):GetClientId() ~= Old then
    while true do end
end
if HWID[table.find(HWID, Old)] == Old then
print("Ok") -- เอา print ออกเอา Src ไส่
--scripthub
else
    setclipboard("HWID : "..tostring(Old))
    game.Players.LocalPlayer:Kick("Wrong Hwid Dm Admin!")
    wait(.5)
    game:Shutdown()
end
