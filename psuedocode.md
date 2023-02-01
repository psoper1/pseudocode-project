## Pseudocode Project

## How to do laundry

## Variables: 
- Rooms (room1, room2, room3, room4, room5) *//These rooms will be checked for clothes*
- laundryRoom *//Where laundry will be completed*
- checkForClothes = checkClothes *//This will be either true or false. True will do the action pickUpClothes. If false, the function will end*
- Clothes *//Object that will be put in to the washingMachine and dryer*
- washingMachine *//Where Clothes will be put in to to wash*
- dryer *//Where Clothes will be put in to dry*
- basketOfClothes = basket *//Where Clothes will be stored while transporting throughout the house and in to the laundryRoom to start wash and dry*
- laundryDetergent = Detergent *//Will be added to the Clothes after Clothes are put in the washingMachine*
- fabricSoftener = Softener *//Will be added to the Clothes after the laundryDetergent is added*
- detergentCap = dCap *//Cap for the laundryDetergent*
- softenerCap = sCap *//Cap for the fabricSoftener*
- washingDial = wDial *//Dial on the washingMachine*
- dryerDial = dDial *//Dial on the dryer*
- washerLid = wLid *//Lid to the washingMachine*
- dryerDoor = dDoor *//Door to the dryer*
- lintTrap *//Lint Trap that will be checked if needed to be clean. Will be two values, true or false. True if > 50% filled and false if < 50% filled*
- lint *//What will be thrown away if found on lintTrap*
- trashCan *//It's a trash can where lint will be put in to if found in lintTrap*
- dryerSlot *//Where the lintTray is found*
- dryerStartButton *//Will start the dryer*

# Go in to each Room
- if Clothes are on the floor
- put clothes in basket
- if there are no clothes
- go to next room until each room has no clothes on the floor (checkForClothes === false)

# Go in to the laundryRoom with the basketOfClothes
- Open lid to washingMachine (washerLid)
- Put Clothes from basketOfClothes in to the washingMachine

# Take cap (dCap) off of laundrDetergent
- Fill cap (dCap) halfway full
- Pour laundryDetergent on the Clothes in one big circle

# Take cap (sCap) off fabricSoftener
- Pour fabricSoftener in to fabaricSpftener compartment until filled
- Put cap (sCap) back on fabricSoftener

# Push and turn dial (wDial) on washingMachine to Normal Wash
- Pull back on dial (wDial) to start the washingMachine
- Place cap (dCap) from laundryDetergent under flowing water until filled
- Pour water from cap (dCap) in to the washingMachine
- Place cap (dCap) back on laundryDetergent

# When the washingMachine has stopped, open washingMachine lid (wLid) (washingMachine.wLid)
-Open the door (dDoor) to the dryer
- If filled with Clothes
- Take Clothes from the dryer and place them in the basketOfClothes that is now empty
- If empty, take Clothes from the washingMachine and place them in to the dryer

# Take out lintTrap
- If lintTrap is > half full, take lint off of lintTrap and place in trashCan
- If l< half full, put lintTrap back in to the dryerSlot
- Close dryer door (dDoor)
- Turn dial (dDial) on the dryer to normal dry
- Press start button (dryerStartButton)

# When the dryer stops, leave Clothes in dryer until either:
- Get the energy to put them away
- Or
- Have to do laundry again