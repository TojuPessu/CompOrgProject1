.data #variables
	ID: .word  02859258
	
	
.text
	li $a0, '@'
	li $v0, 11
	syscall		#calls the system
	sub $v0, $v0, 10
	li, $a0, 0
	syscall
	lw $a0, ID      #loads the word that I stored as my ID
	li $v0, 1
	syscall
	
	li $v0, 11 	#prints out the intergers
	li $a0, 0
	addi $a0, $a0, 10 	#creates a new line following the integer
	syscall
	addi $a0, $a0, 70 	#P( 80)
	syscall
	addi $a0, $a0, 21 	#e (101)
	syscall
	addi $a0, $a0, 14	#s (115)
	syscall 
	addi $a0, $a0, 0 	#s (115)
	syscall
	addi $a0, $a0, 2	#u (117)
	syscall
	sub $a0, $a0, 73	#,(44)
	syscall
	sub $a0, $a0, 12	#space (32)
	syscall
	

	
