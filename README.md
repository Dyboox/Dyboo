# Key System
Dyboo Lib
```local function Start(Key)
	-- your code here
end

local KeySystem = NEVERLOSE:KeySystem("Key System","https://link",function(key)
	if key=='1234' then
		return true
	end
	return false
end)

KeySystem:Callback(Start)```
