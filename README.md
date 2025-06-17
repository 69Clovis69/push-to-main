# push-to-main
tool.hck

-----

# 🌀 YESNO — How to do something

This is a two-line [Befunge-93](https://esolangs.org/wiki/Befunge) program that eternally flips between printing `YES` and `NO`.

Because why not?

## 💡 What It Does

This code:

```befunge
>v"SEY",,_v
^_"ON",,<


 How It Works (If You Must Know)
Starts at the > and moves right.

Redirects down to v, lands on a _ (horizontal IF).

Based on the stack (empty = 0), it goes right, prints NO, and loops back up.

Next time, the stack isn’t empty, so it goes left, prints YES, and loops back down.

------

Running It:
Option 1: Run It Online (Fastest)
Use any online Befunge interpreter:

TIO.run

copy.sh/befunge

Paste in the code and watch the terminal go bonkers.

Option 2: Run Locally with Python
Install a Python Befunge interpreter:

bash
Copy
Edit
pip install befunge93
Save the program as loop.bf.

Run it with this Python script:

python
Copy
Edit
from befunge93 import runfile
runfile("loop.bf")

------

Files
loop.bf – The masterpiece itself

README.md – You're reading it

(optional) run.py – Python launcher if you want to run it locally