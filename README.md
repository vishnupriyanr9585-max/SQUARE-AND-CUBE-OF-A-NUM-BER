# SQUARE AND CUBE OF A NUMBER
# 8051 Square  Program

## AIM
To write and execute an Assembly language program for finding the square of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value to Port 0 (P0).
3. Execute the program.
4. The output square value is stored in Port 2 (P2).

## PROGRAM
```
ORG 0000H
MOV R0,#50#
MOV A,@R0
MOV B,@R0
MUL AB
INC R0
MOV @R0,A
END
```

## OUTPUT
![B1](https://github.com/user-attachments/assets/95fcac49-874a-4185-a3f8-b1802102ef32)


## RESULT
Thus, the square of the given data is calculated using 8051 Keil.

# 8051 Cube  Program

## AIM
To write and execute an Assembly language program for finding the cube of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value.
3. Execute the program.
4. The output cube value is stored in a memory location.

## PROGRAM
```
 MOV RO,#50H; RO → address 50H
 MOV A,@RO; A = value at 50H
 MOV B,A; B = same value
 MUL AB; A*B→ square, result in A(low), B(high)
 MOV B,@RO; B = original value again
 MUL AB; multiply again (A * original value
 INC RO
 MOV @RO,A; store low byte result at 51H
 INC RO
 MOV @RO,B; store high byte result at 52H
 END
```


## OUTPUT
<img width="1686" height="722" alt="Screenshot 2026-02-13 113722" src="https://github.com/user-attachments/assets/87486676-03fe-4e3f-b1f2-7fa9ac6b08df" />

## RESULT
Thus, the cube of the given data is calculated using 8051 Keil.
