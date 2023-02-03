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
- detergentCap =  *//Cap for the laundryDetergent*
- softenerCap =  *//Cap for the fabricSoftener*
- washingDial =  *//Dial on the washingMachine*
- dryerDial =  *//Dial on the dryer*
- washerLid =  *//Lid to the washingMachine*
- dryerDoor =  *//Door to the dryer*
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

 ```js
function checkForClothes {
    if clothes are on the floor in Room
    then true
    else
    then false
};
 ```



# Go in to the laundryRoom with the basketOfClothes
- Open lid to washingMachine (washerLid)
- Put Clothes from basketOfClothes in to the washingMachine

 ```js
function add basketOfClothes to washingMachine;
 ```

# Take cap off of laundrDetergent
- Fill cap halfway full
- Pour laundryDetergent on the Clothes in one big circle

```js
function fill detergentCap to 50%, pour on the Clothes in washingMachine;
```

# Take cap off fabricSoftener
- Pour fabricSoftener in to fabaricSoftener compartment until filled
- Put cap back on fabricSoftener

```js
function take softenerCap off fabricSoftener,
        pour fabricSoftener in to fabricSoftener compartment,
        put softenerCap back on fabricSoftener;
```

# Push and turn dial on washingMachine to Normal Wash
- Pull back on dial to start the washingMachine
- Place cap back on laundryDetergent

```js
        function push washingDial and turn clockwise and break when at Normal Wash,
                pull back on washingDial to start the washingMachine,
                place detergenrCap back on laundryDetergent;
```

# When the washingMachine has stopped, open washingMachine lid (wLid) (washingMachine.wLid)
-Open the door to the dryer
- If filled with Clothes
- Take Clothes from the dryer and place them in the basketOfClothes that is now empty
- If empty, take Clothes from the washingMachine and place them in to the dryer

```js
        function open dryerDoor {
            if has Clothes
            then transfer Clothes from dryer to basketofClothes
            else
            take Clothes from washingMachine and add to dryer
        };
```

# Take out lintTrap
- If lintTrap is > half full, take lint off of lintTrap and place in trashCan
- If < half full, put lintTrap back in to the dryerSlot
- Close dryer door (dDoor)
- Turn dial (dDial) on the dryer to normal dry
- Press start button (dryerStartButton)

```js
function lintTrap {
    if lintTrap > 50%
        then take lint and place in trashCan
    else
        put lintTrap back in dryerSlot
};
```

# When the dryer stops, leave Clothes in dryer until either:
- Get the energy to put them away
- Or
- Have to do laundry again

```js
function Will {
    if will == true
        put Clothes away
    if will == false
        wait until laundry is needed again
};
```

## Code?

```js
function checkForClothes {
    if clothes are on the floor in Room
    then true
    else
    then false
};

function add basketOfClothes to washingMachine;

function fill detergentCap to 50%, pour on the Clothes in washingMachine;

function take softenerCap off fabricSoftener,
        pour fabricSoftener in to fabricSoftener compartment,
        put softenerCap back on fabricSoftener;

function push washingDial and turn clockwise and break when at Normal Wash,
                pull back on washingDial to start the washingMachine,
                place detergenrCap back on laundryDetergent;

function open dryerDoor {
    if has Clothes
        then transfer Clothes from dryer to basketofClothes
    else
        take Clothes from washingMachine and add to dryer
        };

function lintTrap {
    if lintTrap > 50%
       then take lint and place in trashCan
    else
    put lintTrap back in dryerSlot
};

function Will {
    if will === true
        put Clothes away
    if will === false
        wait until laundry is needed again
};

```