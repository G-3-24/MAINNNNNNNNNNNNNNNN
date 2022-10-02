game.StarterGui:SetCore("SendNotification", {
	Title = "AutoClicker";
    Text = "F to turn on and off";
})
SNYPASEWONTUPDATE = false
game:GetService('RunService').Stepped:connect(function()
if SNYPASEWONTUPDATE then
game:GetService("VirtualUser"):ClickButton1(Vector2.new(125,125)) 
end
end)
plr = game.Players.LocalPlayer
mouse = plr:GetMouse()
mouse.KeyDown:connect(function(key)

if key == "f" then
SNYPASEWONTUPDATE = not SNYPASEWONTUPDATE

end
end)
