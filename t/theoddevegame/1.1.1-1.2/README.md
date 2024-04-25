# Comparing `tmp/theoddevegame-1.1.1.tar.gz` & `tmp/theoddevegame-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theoddevegame-1.1.1.tar", last modified: Sat Apr 20 17:46:55 2024, max compression
+gzip compressed data, was "theoddevegame-1.2.tar", last modified: Thu Apr 25 16:33:14 2024, max compression
```

## Comparing `theoddevegame-1.1.1.tar` & `theoddevegame-1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 17:46:55.772860 theoddevegame-1.1.1/
--rw-rw-rw-   0        0        0     2010 2024-04-20 17:46:55.761991 theoddevegame-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-20 17:46:55.774363 theoddevegame-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 17:46:55.714222 theoddevegame-1.1.1/theoddevegame/
-drwxrwxrwx   0        0        0        0 2024-04-20 17:46:55.715648 theoddevegame-1.1.1/theoddevegame/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 17:46:55.759249 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/
--rw-rw-rw-   0        0        0     2010 2024-04-20 17:46:55.000000 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-20 17:46:55.000000 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 17:46:55.000000 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-20 17:46:55.000000 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13989 2024-04-20 17:43:28.000000 theoddevegame-1.1.1/theoddevegame/src/theoddevegame.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:33:14.360885 theoddevegame-1.2/
+-rw-rw-rw-   0        0        0     2004 2024-04-25 16:33:14.358578 theoddevegame-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:33:14.360885 theoddevegame-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 16:33:14.290645 theoddevegame-1.2/theoddevegame/
+drwxrwxrwx   0        0        0        0 2024-04-25 16:33:14.291544 theoddevegame-1.2/theoddevegame/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 16:33:14.358079 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/
+-rw-rw-rw-   0        0        0     2004 2024-04-25 16:33:13.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-25 16:33:13.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:33:13.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 16:33:13.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 16:33:13.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15221 2024-04-25 16:28:27.000000 theoddevegame-1.2/theoddevegame/src/theoddevegame.py
```

### Comparing `theoddevegame-1.1.1/PKG-INFO` & `theoddevegame-1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: theoddevegame
-Version: 1.1.1
-Summary: The digitised odd eve game (The hand cricket version). The version 1.1.1 offers fixes some bugs and minor improvements from v1.1: error in SuperOver.
+Version: 1.2
+Summary: The digitised odd eve game (The hand cricket version). The version 1.2 offers sounds via playsound version 1.2.2
 Author: Prashant Bhatt
 Author-email: pb3924924@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: playsound==1.2.2
 
 
 
 ## The ODD/EVE Game
 
 ODD/EVE is a game in which the player has to throw the numbers and play like cricket.
```

### Comparing `theoddevegame-1.1.1/theoddevegame/src/theoddevegame.egg-info/PKG-INFO` & `theoddevegame-1.2/theoddevegame/src/theoddevegame.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: theoddevegame
-Version: 1.1.1
-Summary: The digitised odd eve game (The hand cricket version). The version 1.1.1 offers fixes some bugs and minor improvements from v1.1: error in SuperOver.
+Version: 1.2
+Summary: The digitised odd eve game (The hand cricket version). The version 1.2 offers sounds via playsound version 1.2.2
 Author: Prashant Bhatt
 Author-email: pb3924924@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: playsound==1.2.2
 
 
 
 ## The ODD/EVE Game
 
 ODD/EVE is a game in which the player has to throw the numbers and play like cricket.
```

### Comparing `theoddevegame-1.1.1/theoddevegame/src/theoddevegame.py` & `theoddevegame-1.2/theoddevegame/src/theoddevegame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Hello everyone, I am Prashant Bhatt, Class XII D of DPS Haldwani, batch 2024-25.
 I made this game the odd eve game, a digitised version of hand cricket.
 So I invite you all to this wonderful game of OddEve. So enjoy.
-This is version 1.1.1 dated 20 April 2024 under MIT License
+This is version 1.2 dated 25 April 2024 under MIT License
 """
 ODDEVE_PICS = ["""
            .-.
            | |
            | |
            | |
     _.-.-.-| | 
@@ -62,44 +62,47 @@
   (____))( \\---
   (____)) _
    (____))
     (__))___/--- """
 ]
 
 import random,time
+from playsound import playsound as ps
 
+lose = "./ono.wav"
+win = "./wd.wav"
+wkt = "./wkt.wav"
 def chance():
     """
     Simulates a toss by asking the user for their preference (odd or even)
     and then randomly choosing a number between 1 and 6 for the program.
 
     Returns:
         True if the user wins the toss (odd + program_number is even), False otherwise.
     """
     print("Here is the toss. Let's go!!!. Choose 'odd' or 'eve(even)'\n")
-    time.sleep(1)
     user_oe=isplayerchance("odd","eve","o","e")
     prog=random.randint(1,6)
     user_tn=validnum()
-    pic(user_tn, "your")
-    pic(prog, "my")
+    pic(user_tn, "Player's")
+    pic(prog, "System's")
     tot=prog+user_tn
     if not user_oe:
         if tot%2!=0:
-            print("You won the toss.")
+            print("Player won the toss.")
             return True
         else:
-            print("I have won the toss")
+            print("System won the toss")
             return False
     else:
         if tot%2==0:
-            print("You have won the toss")
+            print("Player won the toss")
             return True
         else:
-            print("I have won the toss")
+            print("System won the toss")
             return False
 
 def SuperOver():
     """
   Simulates a Super Over when both players are tied in Odd Even Cricket.
 
   This function plays an additional 6 "balls" with the following rules:
@@ -109,51 +112,55 @@
       - Player batting second needs to score 1 run more than the target to win.
   """
     print("\nIt's a tie! Going to Super Over...")
 
   # Player batting first
     player_score = 0
     for i in range(6):
-        print("Your turn:")
+        print("Player's turn:")
         player_number = validnum()
-        print("Now my turn (bowling).")  # Simulate bowling for clarity
+        print("Now System's turn (bowling).")  # Simulate bowling for clarity
         program_number = random.randint(1, 6)
-        pic(player_number, "Your")
-        pic(program_number, "my")
+        pic(player_number, "Player's")
+        pic(program_number, "System's")
         if player_number != program_number:
             player_score += player_number
-            print(f"Your score: {player_score}")
+            print(f"Player's score: {player_score}")
         else:
             player_score += 0
-            print(f"Your score: {player_score}")
+            print(f"System's score: {player_score}")
 
   # Program batting second
     target_score = player_score + 1  # Program needs 1 more than Player's score
     program_score = 0
     for i in range(6):
-        print(f"\nMy turn (target: {target_score}):")
+        print(f"\nSystem's turn (target: {target_score}):")
         program_number = random.randint(1, 6)
-        print("Now your turn (bowling).")  # Simulate bowling for clarity
+        print("Now Player's turn (bowling).")  # Simulate bowling for clarity
         player_number = validnum()
-        pic(player_number, "Your")
-        pic(program_number, "my")
+        pic(player_number, "Player's")
+        pic(program_number, "System's")
         if player_number != program_number:
             program_score += program_number
-            print(f"My score: {program_score}")
+            print(f"System's score: {program_score}")
             if program_score >= target_score:
                 break   # Exit loop if Player 2 reaches or surpasses the target
         else:
             program_score += 0
-            print(f"My score: {program_score}")
+            print(f"System's score: {program_score}")
 
   # Determine winner based on scores
     if program_score > player_score:
-        print(f"Sorry, User! I have won the Super Over and the match! My final score: {program_score}. Your final score: {player_score}. Better luck next time.")
+        print(f"Sorry, Player! System has won the Super Over and the match! System's final score: {program_score}. Player's final score: {player_score}. Better luck next time.")
+        ps(lose)
+        time.sleep(1)
     elif player_score > program_score:
-        print(f"Congratulations! User! You won the Super Over and the match! Your final score: {player_score}. My final score: {program_score}. Keep it up. ")
+        print(f"Congratulations! Player! You won the Super Over and the match! Player's final score: {player_score}. System's final score: {program_score}. Keep it up. ")
+        ps(win)
+        time.sleep(1)
     else:
         print("It's a tie even in the Super Over! We need another Super Over!")
     # Call SuperOver again for another tie-breaker
         SuperOver()
         
 def iscompchance(odd,eve): #if comp won the toss
     """
@@ -163,18 +170,18 @@
         odd: A string displayed as a prompt.
         eve: same as odd.
 
     Returns: boolean values True, False or integral values 0,1.
     """
     c=random.randint(0,1)
     if c==0:
-        print("I will take", eve)
+        print("System takes", eve)
         return 1 
     else:
-        print("I will take", odd)
+        print("System takes", odd)
         return 0
 
 def isplayerchance(odd, eve, o, e):#if player won toss
     """
     Same as iscompchance function, except, it is for user.
     """
     print(odd,"or",eve)
@@ -218,99 +225,117 @@
 def gamelogic(d, point):#the main gamelogic which runs the game.
     """
   Runs the core game loop of Odd Even Cricket until the user quits.
 
   Returns: None
     """
     if d:
-        print("my chance.")#comp. bat first
-        time.sleep(1)
+        print("System's chance.")#comp. bat first
         e=random.randint(1,6)
-        print("I have played my chance, Your turn.")
-        time.sleep(1)
+        print("System has played its chance, Player's turn.")
         f=validnum()
-        pic(e, "my")
-        pic(f, "your")
+        pic(e, "System's")
+        pic(f, "Player's")
         if e==f:#its, out and the chasing starts
             target=point+1
             chase=0
-            print(f"Oh, I got out, you need {target} runs to win \nYour batting.")
+            print(f"Oh, System got out, Player need {target} runs to win \nPlayer's batting.")
+            ps(wkt)
             while chase<target:#while runs are less than required runs keep going
-                time.sleep(1)
                 h=validnum()
-                print("You have played your chance, my turn.")
-                time.sleep(1)
+                print("Player you have played your chance, System's turn.")
                 i=random.randint(1,6)
-                pic(i, "my")
-                pic(h, "your")
+                pic(i, "System's")
+                pic(h, "Player's")
                 if h==i:#batsman out before winning
                     if point==chase:#same point superover starts
                         tx=False
                         SuperOver()
                         break
                     else:
-                        print(f"Sorry, User! I have won the match! by {point-chase} runs. My final score: {point}. Your final score: {chase}. Better luck next time.")
+                        print(f"Sorry, Player! System has won the match! by {point-chase} runs. System's final score: {point}. Player's final score: {chase}. Better luck next time.")
+                        ps(lose)
+                        time.sleep(1)
                         tx=False
                         break
                 else:
                     chase+=h
                     print("target is", target)
-                    print("Now you need",target-chase,"runs")
-                    print("your score is", chase)
+                    print("Now Player, you need",target-chase,"runs")
+                    print("Player's score is", chase)
                     tx=True
             if tx:    
-                print(f"Congratulation, you win, keep it up. My final score: {point}. Your final score: {chase}.")
-                
+                print(f"Congratulation Player, you win, keep it up. System's final score: {point}. Player's final score: {chase}.")
+                time.sleep(0.5)
+                ps(win)
+                time.sleep(1)
         else:
             point+=e
-            print("my score is", point)
+            print("System's score is", point)
             gamelogic(d, point)
             return point
     else:
-        print("your chance.")
-        time.sleep(1)
+        ct=0
+        if 50<=point>=55:
+            if ct==0:
+                print("Player, you have scored a half-century while batting first. Congrats.", ps(win))
+                ct+=1
+        if 100<=point>=105:
+            if ct==1:
+                print("Player, you have scored a century while batting first. Congrats.", ps(win))
+                time.sleep(1)
+                ct+=1
+        if 200<=point>=205:
+            if ct==2:
+                print("Player, you have scored a Double-century while batting first. Congrats.", ps(win))
+                ct+=1
+                time.sleep(2)
+        print("Player's chance.")
         e=validnum()    
-        print("You have played your chance, my turn.")
-        time.sleep(1)
+        print("Player, you have played your chance, Now System's turn.")
         f=random.randint(1,6)
-        pic(e, "your")
-        pic(f, "my")
+        pic(e, "Player's")
+        pic(f, "System's")
         if f==e:
             target=point+1
             chase=0
-            print("Oh, you got out, I need", target, "runs to win \nMy batting")
+            print("Oh, Player you got out, system need", target, "runs to win \nSystem's batting")
+            ps(wkt)
             while chase<target:
-                time.sleep(1)
                 i=random.randint(1,6)
-                print("I have played my chance, your turn.")
-                time.sleep(1)
+                print("System has played its chance, Player's turn.")
                 h=validnum()
-                pic(i, "my")
-                pic(h, "your")
+                pic(i, "System's")
+                pic(h, "Player's")
                 if h==i:
                     if point==chase:
                         tx=False
                         SuperOver()
                         break
                     else:
-                        print(f"Oh, I lost by {point-chase} runs. Congratulation!! Keep it up. My final score is {chase}. Your final score is {point}.")
+                        print(f"Oh, System lost by {point-chase} runs. Congratulation!! Keep it up. System's final score is {chase}. Player's final score is {point}.")
+                        time.sleep(0.5)
+                        ps(win)
+                        time.sleep(1)
                         tx=False
                         break
                 else:
                     chase+=i
                     print("target is ",target)
-                    print("Now I need",target-chase,"runs")
-                    print("my score is", chase)
+                    print("Now System need",target-chase,"runs")
+                    print("System's score is", chase)
                     tx=True
             if tx:
-                print(f"Sorry, User! I have won the match! My final score: {chase}. Your final score: {point}. Better luck next time.")
+                print(f"Sorry, Player! System has won the match! System's final score: {chase}. User's final score: {point}. Better luck next time.")
+                ps(lose)
+                time.sleep(1)
 
         else:
             point+=e
-            print("your score is", point)
+            print("Player's score is", point)
             gamelogic(d, point)
             return point
 
 def rules():
     """
   Prints a detailed explanation of the rules of Odd Even hand Cricket.
     """
```

