local v12=Instance.new("ScreenGui");local v13=Instance.new("Frame");local v14=Instance.new("TextButton");v12.Name="Fly";v12.Parent=game:WaitForChild("CoreGui");v12.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;game:GetService("CoreGui").FlyMobile.Enabled=false;v13.Parent=v12;v13.BackgroundColor3=Color3.fromRGB(1545 -(320 + 1225) ,453 -198 ,0);v13.Position=UDim2.new(0.412993044,0 + 0 ,1464.0562249012 -(157 + 1307) ,1859 -(821 + 1038) );v13.Size=UDim2.new(0,498 -298 ,0 + 0 ,81 -35 );v14.Parent=v13;v14.BackgroundColor3=Color3.fromRGB(95 + 160 ,0 -0 ,1026 -(834 + 192) );v14.Position=UDim2.new(0.0350000001,0 + 0 ,0.0652173907 + 0 ,0 + 0 );v14.Size=UDim2.new(0 -0 ,491 -(300 + 4) ,0 + 0 ,104 -64 );v14.Font=Enum.Font.SourceSans;v14.Text="FLY : OFF";v14.TextColor3=Color3.fromRGB(362 -(112 + 250) ,0,0 + 0 );v14.TextSize=90 -54 ;v14.MouseButton1Down:connect(function()if (_G.flykuy==true) then local v240=0 + 0 ;local v241;local v242;local v243;while true do if (v240==1) then v241.Position=v241.Position + Vector3.new(0,3 + 2 ,0 + 0 ) ;wait(0.5);v241=game.Players.LocalPlayer.Character:FindFirstChild("Collision");v241.Position=v241.Position + Vector3.new(0,5,0 + 0 ) ;v240=2 + 0 ;end if (v240==0) then _G.flykuy=false;getgenv().colfly=false;for v476,v477 in next,game.Players.LocalPlayer.Character:GetDescendants() do if (v477.IsA(v477,"BasePart") and (getgenv().colfly==false)) then v477.CanCollide=true;end end v241=game.Players.LocalPlayer.Character:FindFirstChild("Collision");v240=1415 -(1001 + 413) ;end if (v240==3) then v243=Instance.new("Sound");v243.Parent=game.SoundService;v243.SoundId="rbxassetid://4590657391";v243.Volume=11 -6 ;v240=886 -(244 + 638) ;end if (v240==(695 -(627 + 66))) then v242=nil;function v242(v478)firesignal(game.ReplicatedStorage.EntityInfo.Caption.OnClientEvent,v478);end v242("Fly Disabled");v14.Text="FLY : OFF";v240=3;end if (v240==4) then v243.PlayOnRemove=true;v243:Destroy();break;end end elseif (_G.flykuy==false) then local v319=0 -0 ;local v320;local v321;local v322;while true do if (v319==(603 -(512 + 90))) then getgenv().colfly=true;v320=game.Players.LocalPlayer.Character:FindFirstChild("Collision");v320.Position=v320.Position-Vector3.new(1906 -(1665 + 241) ,722 -(373 + 344) ,0 + 0 ) ;v321=nil;v319=1 + 1 ;end if (v319==(10 -6)) then v322:Destroy();break;end if ((2 -0)==v319) then function v321(v578)firesignal(game.ReplicatedStorage.EntityInfo.Caption.OnClientEvent,v578);end v321("Fly Enabled");v14.Text="FLY : ON";v322=Instance.new("Sound");v319=3;end if ((1099 -(35 + 1064))==v319) then _G.Flykuy=true;v320=game.Players.LocalPlayer.Character:FindFirstChild("Collision");v320.Position=v320.Position-Vector3.new(0 + 0 ,10 -5 ,0 + 0 ) ;wait(0.5);v319=1237 -(298 + 938) ;end if (v319==(1262 -(233 + 1026))) then v322.Parent=game.SoundService;v322.SoundId="rbxassetid://4590657391";v322.Volume=1671 -(636 + 1030) ;v322.PlayOnRemove=true;v319=4;end end end end);
