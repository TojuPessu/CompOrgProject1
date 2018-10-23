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
	
	
