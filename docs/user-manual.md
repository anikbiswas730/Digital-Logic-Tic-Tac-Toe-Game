# Tic-Tac-Toe Digital Logic - User Manual

## Setup Instructions

### Power Supply
1. Connect a regulated 5V DC power supply to the power rails
2. Ensure proper ground connection
3. Check that all ICs receive stable voltage (4.75V - 5.25V)

### Initial Check
- All LEDs should be OFF when powered on
- No LEDs should light up without button presses
- Press RESET button once to ensure clean state

## Playing the Game

### Starting a New Game
1. Power on the circuit or press RESET
2. Player 1 (Red LEDs) always goes first
3. Game board is represented by 9 pushbuttons in 3×3 layout

### Making Moves
1. **Player 1's Turn**: Press any unoccupied button
   - Corresponding position lights up RED
   - Turn automatically switches to Player 2

2. **Player 2's Turn**: Press any unoccupied button
   - Corresponding position lights up GREEN
   - Turn automatically switches to Player 1

3. **Invalid Moves**: The following actions have no effect:
   - Pressing an already occupied button
   - Pressing any button after game ends
   - Pressing buttons during power-up transient

### Winning the Game

The game checks for wins after each move. A player wins by getting three in a row:

**Row Wins**: Positions 1-2-3, 4-5-6, or 7-8-9

**Column Wins**: Positions 1-4-7, 2-5-8, or 3-6-9

**Diagonal Wins**: Positions 1-5-9 or 3-5-7

When a player wins:
- Winner LED lights up (Red or Green)
- All button inputs are disabled
- Game must be reset to play again

### Draw Condition

If all 9 positions are filled with no winner:
- Yellow LED lights up
- No winner LEDs illuminate
- Press RESET to play again

## Button Layout

```
1 | 2 | 3
---------
4 | 5 | 6
---------
7 | 8 | 9
```

## LED Indicators

| LED Color | Meaning |
|-----------|---------|
| Red (Grid) | Player 1's move |
| Green (Grid) | Player 2's move |
| Red (Status) | Player 1 wins |
| Green (Status) | Player 2 wins |
| Yellow (Status) | Draw game |

## Troubleshooting

### Problem: LEDs not lighting up
- Check power supply voltage
- Verify all IC connections
- Check LED polarity
- Ensure resistors are properly connected

### Problem: Wrong player color displayed
- Check player selector circuit connections
- Verify XOR gate inputs
- Press RESET and try again

### Problem: Win not detected
- Verify winner detection circuit wiring
- Check all AND/OR gate connections
- Test with known winning pattern

### Problem: Can't reset game
- Check RESET button connection
- Verify flip-flop clear pins
- Check power supply stability

### Problem: Buttons respond after game ends
- Check game-over signal routing
- Verify AND gate before flip-flops
- Check winner circuit outputs

## Maintenance

- Avoid exceeding 5.5V on any IC
- Keep circuit away from static discharge
- Check for loose connections periodically
- Clean pushbutton contacts if unresponsive

## Technical Support

For circuit diagrams and detailed schematics, refer to the `circuit-diagrams/` folder in the repository.

## Safety Notes

- Use only regulated 5V power supply
- Avoid short circuits
- Handle ICs carefully to prevent static damage
- Disconnect power before making circuit modifications
