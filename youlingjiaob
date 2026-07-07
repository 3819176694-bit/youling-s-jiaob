-- 服务端脚本 (放在 ServerScriptService)
local Players = game:GetService("Players")

-- 方法1：删除所有现有玩家
for _, player in pairs(Players:GetPlayers()) do
    player:Destroy()
end

-- 方法2：监听新玩家并立即删除（持续生效）
Players.PlayerAdded:Connect(function(player)
    player:Destroy()
end)

-- 方法3：清空 Players 容器的所有子项（包括非玩家对象）
-- Players:ClearAllChildren()
