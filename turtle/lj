--Lumber Jack
-- lj <tree size>
-- cut tree of any size
local a = 0
local size = 1
function cut1BlockTree()
	turtle.dig()
	turtle.forward()
	while turtle.detectUp() do
		turtle.digUp()
		turtle.up()
		a = a + 1
	end
	while a > 0 do
		turtle.down()
		a = a - 1
	end
	turtle.back()
	turtle.place()

	end
function cut4BlockTree()
	turtle.dig()
	turtle.forward()
	while turtle.detect() do
		turtle.digUp()
		turtle.dig()
		turtle.up()
		a = a + 1
	end

	turtle.turnLeft()
	turtle.forward()
	turtle.turnRight()

	while a > 0 do
		turtle.digDown()
		turtle.down()
		turtle.dig()
		a = a - 1
	end
	turtle.select(1)
	turtle.place()
	turtle.back()
	turtle.place()
	
	turtle.turnRight()
	turtle.forward()
	turtle.turnLeft()
	turtle.forward()
	turtle.place()
	turtle.back()
	turtle.place()
end
function say(Str)
	print(Str)
end
function splashScreen()
	shell.run('clear')
	say("Redwood LumberJack v0.1")
	say("=======================")
	say("")
	say("Turtle should be placed next to a readwood tree.")
	say("press Ctrl-T and hold to terminate")

end

--display welcome screen
splashScreen()
if #args == 1 then
	size = tonumber(args[1])
else
	print( "Usage: lj <tree size>" )
	return
end

if size < 1 then
	print( "tree footprint must be positive" )
	return
end
if size == 1 then
	cut1BlockTree()
elseif size == 4 then
	cut4BlockTree()
end

say("GoodBye")