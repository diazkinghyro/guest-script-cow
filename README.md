gg.setVisible(false)

gg.clearResults()

gg.clearList()

local guest = {'10283','10282','10264','16118'}

local time = os.date('%H%M')

local x = "0"

local y = "0"

pkgname = gg.getTargetPackage()

required = "com.extremedevelopers.codeofwar"

if pkgname ~= required then gg.alert("\n⚠️ SOMETHING WENT WRONG! ⚠️\n\n— SCRIPT INAPPROPRIATE APP ISSUE")

return
end

App = gg.getTargetInfo()

expiration = "20230106"

date = os.date("%Y%m%d")

if expiration <= date then

return

end

if date == '02232022' then

gg.alert('\nℹ️ NEW ADDITIONAL FEATURES WILL BE COME SOON ℹ️\n\n— ADMIN')

end

gg.toast('Verifying, please wait...')

gg.sleep(1000)

gg.toast('Verifying, please wait.')

gg.sleep(1000)

gg.toast('Verifying, please wait..')

gg.sleep(1000)

gg.toast('Verifying, please wait...')

gg.sleep(1000)

for l , I in pairs(guest) do
if App.uid == I then A = true end
end
if A ~= true then

gg.toast('Something went wrong!')

gg.sleep(1000)

gg.alert("\n⚠️ YOUR DEVICE IS NOT REGISTERED ⚠️\n\n— YOUR ID NO. :"..App.uid)

return

else

gg.toast('DEVICE REGISTERED')

gg.sleep(1500)

end

if time >= "0400" and time <= "0800" then

gg.alert('\n** GOOD MORNING!\n\n— TAKE A BREAKFAST BEFORE PLAY.')

end

if time >= "1100" and time <= "1300" then

gg.alert('\n** GOOD AFTERNOON!\n\n— TAKE A LUNCH BEFORE PLAY.')

end

if time >= "1800" and time <= "2100" then

gg.alert('\n** GOOD EVENING!\n\n— TAKE A DINNER BEFORE PLAY.')

end

if time >= "0000" and time <= "0300" then

gg.alert('\nHEY BROTHER, YOU BETTER GET SOME REST!')

end

if time >= x and time <= y then

gg.alert('\n✅ YOU ARE AUTOMATICALLY BYPASSED!\n\n** NO ANY PASSWORD\n\n— ADMIN')

goto START

end

::ADMIN::

pass = gg.prompt({"ENTER THE ADMINISTRATOR PASSWORD:","GUEST PASSWORD (PLEASE CHECK, IF YOU ARE GUEST)"},{},{[1]='text',[2]='checkbox'})

if pass == nil then goto ADMIN end

if pass[2] == true then goto XGUEST end

if pass[1] == "" then gg.alert('\n⚠️ NO INPUT ENTERED! ⚠️') goto ADMIN end

pass = pass[1]..' '
allowed = false
function allow_password(password)
	if password..' ' == pass then 
		allowed = true
	end
end

allow_password('$admin')
allow_password('#king22')

if not allowed then

	gg.alert('\n⚠️ INCORRECT PASSWORD ENTERED! ⚠️')

goto ADMIN

else 

	gg.alert("\n✅ You have successfully entered the script!\n\n— Enjoy!")

goto START

end

::XGUEST::

gg.toast('Generating password, please wait...')

gg.sleep(2000)

gg.toast('Generating password, please wait.')

gg.sleep(2000)

gg.toast('Generating password, please wait..')

gg.sleep(2000)

gg.toast('Generating password, please wait...')

gg.sleep(2000)

gg.toast('Done!')

gg.sleep(2000)

day = os.date('%d')

year = os.date('%Y')

hour = os.date('%I')

minute = os.date('%M')

second = os.date('%S')

code = math.random(1000000, 9999999)

guestpass = gg.prompt({"ENTER YOUR PASSWORD AS GUEST:\n\n"..code.."","Approved by Admin"},{},{[1]='text',[2]='checkbox'})

if guestpass == nil then

gg.alert('\n⚠️ NO INPUT ENTERED! ⚠️')

goto XGUEST

end

if guestpass[2] == false then gg.alert('\n⚠️ PLEASE CHECKED ADMIN APPROVAL ⚠️') goto XGUEST end

if guestpass[1] == "" then gg.alert('\n⚠️ INCORRECT PASSWORD ENTERED! ⚠️') goto XGUEST end

guestpass = guestpass[1]..' '
allowed = false
function allow_password(password)
	if password..' ' == guestpass then 
		allowed = true
	end
end

allow_password(code)

if not allowed then

gg.alert('\n⚠️ INCORRECT PASSWORD ENTERED! ⚠️')

goto XGUEST

else

	gg.alert("\n✅ You have successfully entered the script!\n\n— Enjoy!") goto START end

::START::

gg.alert('\n\n\t\t\t\t\t\t\t\t\t\t\tThis hackscript only for Code Of War')

gg.alert('" Be a Advanced gamer using my hack-script. "\n\n@Lord-King')

letters = {'q','w','e','r','t','y','u','i','o','p','a','s','d','f','g','h','j','k','l','z','x','c','v','b','n','m','Q','W','E','R','T','Y','U','I','O','P','A','S','D','F','G','H','J','K','L','Z','X','C','V','B','N','M','1','2','3','4','5','6','7','8','9','0'}

length = math.random(2, 4)

text = ""

for i = 1,length do


text = text.. "" ..letters[math.random(1,#letters)]

if i == length then

name = {text}

time = time..""

x = x..""

y = y..""

if time >= x and time <= y then

goto PASS

end

if pass[1] == password then

goto PASS

end

::CODE::

Menu = gg.prompt({'ENTER THE ('..length..') GIVEN CODE TO UNLOCK:\n\n'..text..''},nil,{"text"})

if Menu == nil then

gg.sleep(1500)

goto CODE

end

if Menu[1] == "" then gg.alert('\n⚠️ NO INPUT ENTERED! ⚠️') goto CODE end

if not Menu then return end
for l , I in pairs(name) do
if Menu[1] == I then A = true end
end
if A ~= true then

gg.alert('\n⚠️ INCORRECT PASSWORD ENTERED! ⚠️')

gg.sleep(3000)

goto CODE

else

gg.sleep(500)

gg.toast("Correct!")

end

::PASS::

gg.sleep(500)

gg.setRanges(gg.REGION_C_ALLOC | gg.REGION_ANONYMOUS)

gg.setVisible(false)

gg.toast('Scanning...')

gg.sleep(1000)

gg.toast('Please wait and be patience')

gg.startFuzzy()

gg.toast('Found address: *'..gg.getResultsCount())

gg.clearResults()

gg.clearList()

gg.sleep(1000)

gg.toast('READY TO ROCK!')

gg.sleep(1000)

gg.toast('This hackscript by @Lord-King')

gg.sleep(1500)

::BULLET::

local xb = gg.prompt({'~Enter exact amount of your bullet.\n\nExample: "10, 20, 30" per magazine.'},nil,{'number'})

if xb == nil then goto BULLET end

if xb[1] ~= '10' and xb[1] ~= '20' and xb[1] ~= '25' and xb[1] ~= '30' and xb[1] ~= '60' then

gg.alert('\n— PLEASE ENTER THE EXACT AMOUNT.')

goto BULLET

end

gg.toast(xb[1])

gg.sleep(1500)

::SPEED::

local xspeed = gg.prompt({'Set your speed level\n[5; 30]'},{15},{'number'})

if xspeed == nil then goto SPEED end

gg.toast(xspeed[1])

gg.sleep(1500)

::XMENU::

XMENU = gg.prompt({'PLEASE TURN IT ON YOUR DESIRED OPTIONS\n\nENABLE = 1                |                DISABLE = 0\n---------------------------------------------------------------------------\nNO RECOIL + NO RELOAD[0; 1]','\nSPEED HACK[0; 1]','\nQUICK RESPAWN FOR FFA[0; 1]'},nil,{'number','number','number'})

if XMENU == nil then

gg.alert('⚠️ INVALID INPUT! ⚠️\n\n—PLEASE TURN IT ON YOUR DESIRED OPTIONS!')

gg.sleep(1000)

goto XMENU

end

gg.toast('Please wait...')

gg.sleep(1500)

local dword = gg.TYPE_DWORD

local float = gg.TYPE_FLOAT

------------- MAIN CODE --------------

function WH()

local t = gg.getListItems()
gg.loadResults(t)

end

function HIDE()

gg.toast('Press x-gamer tools to open again.')

gg.setVisible(false)
while true do
    if gg.isVisible() then
        gg.setVisible(false)
      break
    end
    gg.sleep(100)
end

return Main()

end

function Main()
local menu=gg.choice({'>> START SCRIPT','>> ABOUT'},nil, '----------------- SIMPLE HACK -----------------\n--------------- LORDKINGDIAZ ----------------')

if menu==nil then HIDE() end
if menu == 1 then START() end
if menu == 2 then ABOUT() end

end

function START()

if XMENU[1] == '1' then

gg.clearResults()

gg.setRanges(gg.REGION_ANONYMOUS)

gg.searchNumber(xb[1]..'D;0D;0D;0D;1D::17', dword)

gg.refineNumber(xb[1], dword)

gg.refineAddress('??8', 0xFFF)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

    values[#values + 1] = {address = results[i].address - 0x1C, flags = dword}
    
  end

gg.loadResults(values)

gg.refineNumber('100~150', dword)

gg.refineAddress('??C', 0xFFF)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

    values[#values + 1] = {address = results[i].address + 0x4, flags = dword}
    
  end

gg.loadResults(values)

gg.refineAddress('??0', 0xFFF)

gg.refineNumber('1~30', dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

    values[#values + 1] = {address = results[i].address - 0x0, flags = dword, value = 29, freeze = true}
values[#values + 1] = {address = results[i].address + 0x4, flags = float, freeze = true}
values[#values + 1] = {address = results[i].address + 0x8, flags = float, freeze = true}
    
  end
  
gg.addListItems(values)   -- // OFFSET END

gg.loadResults(values)

if gg.getResultsCount()<=0 then gg.toast('Something went wrong!') end

if gg.getResultsCount()>0 then gg.toast('No recoil + No reload activated!') end

gg.clearResults()

end

if XMENU[2] == '1' then

gg.clearResults()

gg.setRanges(gg.REGION_C_ALLOC)   -- // SPEED-HACK

gg.searchNumber(65793, dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

values[#values + 1] = {address = results[i].address + 0x4, flags = dword}
values[#values + 1] = {address = results[i].address + 0x8, flags = dword}
values[#values + 1] = {address = results[i].address + 0x10, flags = dword}
values[#values + 1] = {address = results[i].address + 0x18, flags = dword}
values[#values + 1] = {address = results[i].address + 0x1C, flags = dword}
values[#values + 1] = {address = results[i].address + 0x20, flags = dword}
values[#values + 1] = {address = results[i].address + 0x28, flags = dword}
    
  end

gg.loadResults(values)

gg.refineNumber('27D;1D;0D;2D;4D::25', gg.TYPE_DWORD)

gg.refineNumber(27, dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

values[#values + 1] = {address = results[i].address - 0x14, flags = float}

end

gg.loadResults(values)

local y = gg.getResults(999)

if xspeed[1] >= '5' and xspeed[1] <= '9' then

gg.editAll('1.0'..xspeed[1], gg.TYPE_FLOAT)

end

if xspeed[1] >= '10' and xspeed[1] <= '30' then

gg.editAll('1.'..xspeed[1], gg.TYPE_FLOAT)

end

gg.addListItems(y)

if gg.getResultsCount()<=0 then gg.toast('Something went wrong!') end

if gg.getResultsCount()>0 then gg.toast('Speed-hack activated!') end  

gg.clearResults()

end

return HIDER()

end

function ABOUT()

gg.sleep(500)

local about = "\n[=== CODE OF WAR HACK ===]\n\n< FEATURES >\n\n>> NO RECOIL + NO RELOAD\n\n>> SPEED-HACK\n\n>> QUICK RESPAWN [FFA]\n\n+++ < ADDITIONAL FEATURES > +++\n\n>> [CHANGE SPEED-HACK IN BATTLE]\n\n--------------------------------------------------------------------------------------------\n\n### This hackscript by Lord-King ###\n\n### Educational purposes only ###"

gg.alert(about)

gg.sleep(1000)

return HIDEE()

end

function HIDER()

gg.sleep(1000)

gg.toast('Press x-gamer tools to open again.')

gg.setVisible(false)
while true do
    if gg.isVisible() then
        gg.setVisible(false)
      break
    end
    gg.sleep(100)
end

return RESETM()

end

function RESETM()
local menu=gg.choice({'>> RE-ACTIVATE NO RECOIL + NO RELOAD','>> QUICK RESPAWN [FFA ONLY]','>> CHANGE GAME SPEED','>> SAFE MODE'},nil, '---------- SAFE MODE ----------\n-------- LORDKINGDIAZ --------')

if menu == nil then HIDER() end
if menu == 1 then NR() end
if menu == 2 then FFA() end
if menu == 3 then NSPEED() end 
if menu == 4 then RESET() end



end

function NR()

if XMENU[1] == '0' then

gg.toast('Please enabled this option first')

gg.sleep(2000)

return HIDER()

end

gg.clearResults()

local dword = gg.TYPE_DWORD

local float = gg.TYPE_FLOAT

gg.setRanges(gg.REGION_ANONYMOUS)

gg.searchNumber(xb[1], dword)

local count = gg.getResultsCount()

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

values[#values + 1] = {address = results[i].address + 0x10, flags = dword}

end

gg.loadResults(values)

gg.refineNumber('16,777,000~16,777,999', dword)


local count = gg.getResultsCount()

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do


values[#values + 1] = {address = results[i].address + 0x4, flags = dword}

end

gg.loadResults(values)

gg.refineNumber('1~999', dword)

local count = gg.getResultsCount()

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

values[#values + 1] = {address = results[i].address - 0x30, flags = dword}

end

gg.loadResults(values)

gg.refineNumber('100~150', dword)

local count = gg.getResultsCount()

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

values[#values + 1] = {address = results[i].address + 0x4, flags = dword}

end

gg.loadResults(values)

gg.refineNumber('1~30', dword)

gg.refineAddress('??0', 0xFFF)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do

    values[#values + 1] = {address = results[i].address - 0x0, flags = dword, value = 29, freeze = true}
values[#values + 1] = {address = results[i].address + 0x4, flags = float, freeze = true}
values[#values + 1] = {address = results[i].address + 0x8, flags = float, freeze = true}
    
  end

if gg.getResultsCount()>0 then gg.toast('Fire-power activated!') end
  
gg.addListItems(values)   -- // OFFSET END

gg.loadResults(values)

gg.clearResults()

return HIDER()

end

function FFA()

if XMENU[3] == '0' then

gg.toast('Please enabled this option first')

gg.sleep(2000)

return HIDER()

end

if XMENU[3] == '1' then

gg.clearResults()

gg.setRanges(gg.REGION_ANONYMOUS)

WH()

gg.refineNumber(0, dword)

gg.refineAddress('??0', 0xFFF)

if gg.getResultsCount()>0 then

local count = gg.getResultsCount()

local results = gg.getResults(count)

for i , v in ipairs(results) do

v.freeze = false

end

gg.addListItems(results)

gg.clearResults()

gg.toast('Disable quick respawn!')

end

gg.toast('Press again later')

gg.setVisible(false)
while true do
    if gg.isVisible() then
        gg.setVisible(false)
      break
    end
    gg.sleep(100)
end

gg.toast('Scanning...')

gg.sleep(1000)

gg.toast('Please wait and be patience')

local dword = gg.TYPE_DWORD

local float = gg.TYPE_FLOAT

gg.setRanges(gg.REGION_ANONYMOUS)

gg.searchNumber(10, dword)

gg.refineAddress('??C', 0xFFF)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do


    values[#values + 1] = {address = results[i].address - 0x28, flags = dword}


  end

gg.loadResults(values)

gg.refineNumber('100~150', dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do


    values[#values + 1] = {address = results[i].address + 0x20, flags = dword}


  end

gg.loadResults(values)

gg.refineNumber('100~150', dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do


    values[#values + 1] = {address = results[i].address + 0x4, flags = dword}


  end

gg.loadResults(values)

gg.refineNumber(1, dword)

local count = gg.getResultsCount()   -- // OFFSET START

local results = gg.getResults(count)

local values = {}

for i, v in pairs(results) do


    values[#values + 1] = {address = results[i].address + 0x8, flags = dword}


  end

gg.loadResults(values)

gg.refineNumber('0~10', dword)

gg.refineAddress('??0', 0xFFF)

local count = gg.getResultsCount()

local results = gg.getResults(count)

for i, v in pairs(results) do

v.value = "0"
v.freeze = true

end

gg.addListItems(results)

gg.toast('Found address: *'..gg.getResultsCount())

gg.sleep(500)

if gg.getResultsCount()<=0 then gg.toast('Something went wrong!') end

if gg.getResultsCount()>0 then gg.toast('Instant respawn activated!') end

gg.clearResults()

end

return HIDER()

end

function NSPEED()

if XMENU[2] == '0' then

gg.toast('Please enabled this option first')

gg.sleep(2000)

return HIDER()

end

gg.clearResults()

WH()

gg.refineNumber('1~2', gg.TYPE_FLOAT)

if gg.getResultsCount()<=0 then gg.toast('Something went wrong!') gg.sleep(500) HIDER() return end

local xv = gg.getResultsCount()

local v = gg.getResults(xv)

local value = v[1].value

gg.toast('Current speed: '..value)

local speed = gg.prompt({'Adjust your player speed\n[5; 30]'},{15},{'number'})

if speed == nil then return HIDER() end

gg.getResults(999)

if speed[1] >= '5' and speed[1] <= '9' then

gg.editAll('1.0'..speed[1], gg.TYPE_FLOAT)

end

if speed[1] >= '10' and speed[1] <= '30' then

gg.editAll('1.'..speed[1], gg.TYPE_FLOAT)

end

if gg.getResultsCount()>0 then gg.toast('Done!') gg.sleep(100) end

gg.clearResults()

return HIDER()

end

function RESET()

gg.clearList()

gg.clearResults()

local dword = gg.TYPE_DWORD

local float = gg.TYPE_FLOAT

WH()

local x = gg.getResults(999)

local count = gg.getResultsCount()   -- // OFFSET START


local results = gg.getResults(count)

for i, v in pairs(results) do

v.freeze = "false"

    
  end

gg.loadResults(results)

gg.refineNumber(0, dword)

gg.getResults(999)

gg.editAll(99999, dword)

gg.clearResults()

gg.loadResults(results)

gg.refineNumber('1~2', float)

gg.getResults(999)

gg.editAll(1, float)

gg.clearResults()

gg.clearList()

gg.loadResults(x)

gg.refineNumber('0~~0', dword)

gg.getResults(999)

gg.editAll(99999, dword)

gg.clearList()

gg.clearResults()

return HIDE()

end

--------- END MAIN CODE ----------

while(true)do

if HIDE() then
gg.setVisible(false)
HIDE()

end
end

end
end
