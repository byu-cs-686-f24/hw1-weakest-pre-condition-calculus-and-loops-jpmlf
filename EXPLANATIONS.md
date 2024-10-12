hw1 weakest precondition calculus and loops
James Fitzgerald
Question 1
	Post condition
		Q=(0≤y)∧(0≤x⇒y=x)∧(x<0⇒y=−x)
	If else B=(x<0)
		WP(if B then S1 else S2,Q)=(B⇒WP(S1,Q))∧(¬B⇒WP(S2,Q))
	Substitute
		((x<0)⇒(0≤-x)∧(0≤x⇒-x=x)∧(x<0⇒-x=−x))
        ∧((0≤x)⇒(0≤x)∧(0≤x⇒x=x)∧(x<0⇒x=−x))
	Simplify
		((x<0)⇒(x≤0)∧(0≤x⇒−x=x)∧(x<0⇒−x=−x))
        ∧((0≤x)⇒(0≤x)∧(0≤x⇒x=x)∧(x<0⇒x=−x))
	TRUE
Question 2
	Part 1
	Post condition 
		Q= big>small
	If else x>y
		WP(if B then S1 else S2,Q)=(B⇒WP(S1,Q))∧(¬B⇒WP(S2,Q))
	Substitute {big, small := x, y} in the then and {big, small := y, x;} in the else
		((x>y) ⇒(x>y))
∧((x≤y) ⇒(y>x))
	The precondition fails because (x≤y) can be true at the same time that  (y>x) is false
	So x != y ==> wp(S,Q)
	Part 2
	 
Question 3
	Part A
		Post condition
			Res = n0 * m0
		Loop invariant
			I: res + n * m == n0 * m0
		 
	Part B
		
Question 4
	Part A
	 
	Part B
		
	
