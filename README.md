memFrom, memTo, lib, num, lim, results, src, ok = 0, -1, nil, 0, 32, {}, nil, false function name(n) local srd = gg;if lib ~= n then lib = n ranges = srd.getRangesList(lib) if #ranges == 0 then gg.toast("ᴄᴏɴᴇᴄᴛᴇsᴇ ᴀ ғʀᴇᴇ ғɪʀᴇ ᴘᴀʀᴀ ᴘᴏᴅᴇʀ ᴇᴊᴇᴄᴜᴛᴀʀ ᴇʟ sᴄʀɪᴘᴛ") gg.setVisible(true) os.remove(gg.EXT_STORAGE .. "/Android/data/com.dts.freefireth/files/reportnew.db", gg.LOAD_APPEND) os.remove(gg.EXT_STORAGE .. "/Android/data/com.dts.freefireth/files/ymrtc_log.txt", gg.LOAD_APPEND) print("\n🚫Error 🛇==ᴅᴇ ᴇᴊᴇᴄᴜᴄɪᴏɴ ɴᴜʟʟ🛠\n⚠ᴘᴀʀᴀ ᴀᴄᴛɪᴠᴀʀ ᴇɴᴛʀᴀʀ ᴀʟ ᴊᴜᴇɢᴏ ᴘʀɪᴍᴇʀᴏ⚠") os.exit() else memFrom = ranges[1].start memTo = ranges[#ranges]['end'] end end end function hex2tbl(hex) ret = {} hex:gsub('%S%S', function (ch) ret[#ret + 1] = ch return '' end) return ret end function original(orig) tbl = hex2tbl(orig) len = #tbl if len == 0 then return end used = len if len > lim then used = lim end s = '' for i = 1, used do if i ~= 1 then s = s..';' end v = tbl[i] if v == '??' or v == '**' then v = '0~~0' end s = s..v..'r' end s = s..'::'..used gg.searchNumber(s, 1, false, gg.SIGN_EQUAL, memFrom, memTo) if len > used then for i = used + 1, len do v = tbl[i] if v == '??' or v == '**' then v = 256 else v = ('0x'..v) + 0 if v > 127 then v = v - 256 end end tbl[i] = v end end found = gg.getResultCount(); results = {} count = 0 checked = 0 while true do if checked >= found then break end all = gg.getResults(8) total = #all start = checked if checked + used > total then break end for i, v in ipairs(all) do v.address = v.address + myoffset end gg.loadResults(all) while start < total do good = true offset = all[1 + start].address - 1 if used < len then get = {} for i = lim + 1, len do get[i - lim] = {address = offset + i, flags = 1, value = 0} end get = gg.getValues(get) for i = lim + 1, len do ch = tbl[i] if ch ~= 256 and get[i - lim].value ~= ch then good = false break end end end if good then count = count + 1 results[count] = offset checked = checked + used else del = {} for i = 1, used do del[i] = all[i + start] end gg.removeResults(del) end start = start + used end end end function replaced(repl) num = num + 1 tbl = hex2tbl(repl) if src ~= nil then source = hex2tbl(src) for i, v in ipairs(tbl) do if v ~= '??' and v ~= '**' and v == source[i] then tbl[i] = '**' end end src = nil end cnt = #tbl set = {} s = 0 for _, addr in ipairs(results) do for i, v in ipairs(tbl) do if v ~= '??' and v ~= '**' then s = s + 1 set[s] = { ['address'] = addr + i,  ['value'] = v..'r', ['flags'] = 1,} end end end if s ~= 0 then gg.setValues(set) end ok = true end
-----------------------------SECURITY CODE END-------------------------------
function AYTOUS(Offset, Replaced)  --il2cpp
    Replaced = Replaced:gsub("..",function(c)
    c = c.." "
    return c
    end)
    gg.clearResults()
    gg.setRanges(gg.REGION_CODE_APP | gg.REGION_C_DATA)
    name("libil2cpp.so")
    myoffset = Offset
    original("7F 45 4C 46 01 01 01 00")
    replaced(Replaced)
    for i=1,math.random(50,100) do
        gg.clearResults()
    end
end 

------------

-------------١------------"
gg.alert("🇹🇳يمكنك استخدام حسابك في هذا السكربت لان لايوجد فيه بلاك ليست و لا باند")
gg.alert("You Can use your account because this script no Black list and Ban 🇺🇸")
function START()
vip = gg.choice({
"🛑FIRE PASS NOMOR",
"🛑BOOYAH!", 
"🛑MONY", 
"🛑SIII", 
"🛑ONE PUNCH MAN",
"🛑BOX", 
"🛑ZOMBI", 
"🛑FARA3INA", 
"🛑BOMBA",
"🛑LKAF",
"🛑MOTOR",
"🛑CAR",
"🛑9ALEYA",
"🛑MOCO",
"🛑BATRI9",
"🛑KUNGFU TIGRES",
"🛑BEATBOX",
"🛑L3ALAM",
"🛑NAR",
  "⛔EXIT⛔"
 },nil,"Youtube : BLRX CHI5              EXPIRE DATE : 9999999 DAYS 😀")
 
if vip == nil then else end
 if vip == 1 then FOR1() end
 if vip == 2 then FOR2() end
 if vip == 3 then FOR3() end
 if vip == 4 then FOR4() end
 if vip == 5 then FOR5() end
 if vip == 6 then FOR6() end
 if vip == 7 then FOR7() end
 if vip == 8 then FOR8() end
 if vip == 9 then FOR9() end
 if vip == 10 then FOR10() end
 if vip == 11 then FOR11() end
 if vip == 12 then FOR12() end
 if vip == 13 then FOR13() end
 if vip == 14 then FOR14() end
 if vip == 15 then FOR15() end
 if vip == 16 then FOR16() end
 if vip == 17 then FOR17() end
 if vip == 18 then FOR18() end
 if vip == 19 then FOR19() end
 if vip == 20 then FOR20() end
 if vip == 22 then Exit() end
 menuk = -1
 end
  function FOR1()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000017", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR2()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000060", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR3()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000038", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR4()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000066", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR5()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000067", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR6()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000079", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR7()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000016", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR8()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000011", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR9()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000012", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR10()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000025", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR11()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000074", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR12()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000088", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR13()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000091", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR14()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000093", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR15()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000095", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR16()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000144", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR17()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000126", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR18()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000128", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function FOR19()
    gg.setRanges(gg.REGION_ANONYMOUS)
    gg.searchNumber("909000000~909000145", gg.TYPE_DWORD)
    gg.getResults("100000")
    gg.editAll("909000133", gg.TYPE_DWORD)
    gg.clearResults()
    gg.toast("💡ON💡")
  end
function Exit()  
  print("☆☆")
  print("         ")
  print("    L      ")
  print("     ")
  print("    PLZ ")
  print("  ")
  print(".")
  print("❣️")
  print(" ❤️")
 
os.exit()
end
 
while true do
  if gg.isVisible(true) then
    menuk = 1
    gg.setVisible(false)
  end
  if menuk == 1 then
    START()
  end
  if menu == 2 then
      START()
    end
  menuk = -1
end
