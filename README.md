Setting_Farm :AddToggle({
    Name = "Bring Mob",
	Value = true,
    Callback = function(t)
		_G.Brimob = t
	end
})

spawn(function()
	while wait() do
		if _G.Brimob then
			_G.BringNormal = false
			wait(0.5)
			_G.BringNormal = true
			wait(0.5)
		end
	end
end)
function InMyNetWork(object)
	if isnetworkowner then
		return isnetworkowner(object)
	else
		if (object.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 200 then 
			return true
		end
		return false
	end
end
spawn(function()
	while true do wait()
		if setscriptable then
			setscriptable(game.Players.LocalPlayer, "SimulationRadius", true)
		end
		if sethiddenproperty then
			sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
		end
	end
end)
spawn(function()
	while task.wait() do
		pcall(function()
			if _G.Brimob and _G.BringNormal and hitler then
				for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
					if not string.find(v.Name,"Boss") and (v.HumanoidRootPart.Position - PosMon.Position).magnitude <= 500 then
						if InMyNetWork(v.HumanoidRootPart) then
							v.HumanoidRootPart.CFrame = PosMon
							v.Humanoid.JumpPower = 0
							v.Humanoid.WalkSpeed = 0
							v.HumanoidRootPart.Size = Vector3.new(60,60,60)
							v.HumanoidRootPart.Transparency = 1
							v.HumanoidRootPart.CanCollide = false
							v.Head.CanCollide = false
							if v.Humanoid:FindFirstChild("Animator") then
								v.Humanoid.Animator:Destroy()
							end
							v.Humanoid:ChangeState(11)
							v.Humanoid:ChangeState(14)
							sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius",  math.huge)
						end
					end
				end
			end
		end)
	end
end)

require(game.ReplicatedStorage.Util.CameraShaker):Stop()






local Code = {
			"CINCODEMAYO_BOOST",
			"15B_BESTBROTHERS",
			"Sub2CaptainMaui",
			"DEVSCOOKING",
			"NOOB_REFUND",
			"kittgaming",
			"Sub2Fer999",
			"Enyu_is_Pro",
			"Magicbus",
			"JCWK",
			"Starcodeheo",
			"Bluxxy",
			"fudd10_v2",
			"SUB2GAMERROBOT_EXP1",
			"Sub2NoobMaster123",
			"Sub2UncleKizaru",
			"Sub2Daigrock",
			"Axiore",
			"TantaiGaming",
			"StrawHatMaine",
			"Sub2OfficialNoobie",
			"Fudd10",
			"Bignews",
			"TheGreatAce",
            "SECRET_ADMIN",
            "KITT_RESET",
            "Sub2CaptainMaui",
            ""
		}
		
		spawn(function()
			for _, code in ipairs(Code) do
				game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Redeem"):InvokeServer(code)
				wait()
			end
		end)


Fast atack
  https://raw.githubusercontent.com/XeroxSp/Kobennobbbbbbb/main/README.md
