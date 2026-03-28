# Fix-errors
try to dump all files with entire output
+ try to do 100% unc and env
Sometimes it confuses a loadstring and assigns it as a local library when it should be a normal one. I just want it to detect if it's a library or not. If it is a library, assign it as local; if not, don't assign it as local library. 
Output not generated: [string "Obfuscated_Script"]:1: <name> expected near 'nil'
Add dump with code block example: .l ```print("hi")```
Output not generated: [string "Obfuscated_Script"]:455: unexpected symbol near ':'
Output not generated: [string "Obfuscated_Script"]:1: 'until' expected near 'end'
Output not generated: [string "Obfuscated_Script"]:1: control structure too long near 'end'
Try to dump thid aswell:
https://gitlab.com/rlbx-scripts/elysium-sab/-/raw/main/elysium-sab
if the bot detects @everyone or @here put that he dosent write that in the output or message because it could get spammed the bot need to skip @pings 
___
parchea estos detections
```lua
local Players = game:GetService('Players')
local rat = 0 

for _,v in pairs(Players:GetPlayers()) do
  rat = rat + 1
end

if rat == 0 then
  error('env logger')
  while true do task.wait() end
end

print('pass')
``````lua
local HttpService = game:GetService('HttpService')
local encoded = HttpService:JSONEncode({emageontop = true})

if not HttpService:JSONDecode(encoded).emageontop then
    error('env logger')
    while true do task.wait() end
end

print('pass')
``````lua
sigmaemage = function() return "ratted" end

if iscclosure(sigmaemage) then
    error('env logger')
    while true do task.wait() end
end

print('pass')
``````lua
local test = Instance.new('Part')

if type(test) ~= 'userdata' then
  error('is this ud?')
  while true do task.wait() end
end

print('pass')
``````lua
local suc, dih = pcall(function()
    local test = Instance.new('Part')
    test.CFrame = 6767
end)

if suc then
    error('env logger')
    while true do task.wait() end
end

print('pass')
``````lua
local suc, dih = pcall(function()
  Instance.new('Part'):FireServer()
end)

if suc then
  error'env logger'
  while true do task.wait() end
end

print('pass')
```
