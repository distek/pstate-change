# pstate-change
Bash script to change the pstate of Nvidia cards when using the **Nouveau** driver

## Usage
Requires root/sudo access.

Your output might be different than what you see below.

```
Usage:
	pstate-change [option number]

Options:
(* == current)
	0) 07: core 405 MHz memory 810 MHz
	1) 0a: core 270-1124 MHz memory 1600 MHz
	2) 0f: core 270-1124 MHz memory 5010 MHz *
	3) AUTO
```

## Installation

EZPZ

Copy it to a directory in your $PATH:

```
git clone https://github.com/distek/pstate-change.git
cd pstate-change
cp pstate-change /path/in/your/$PATH/variable/
```

## Running
A few options:
- Add the path to the script (i.e `/usr/local/bin/pstate-change`) to the sudoers file:
  - `%wheel ALL=(ALL) NOPASSWD: /usr/local/bin/pstate-change`
  - This allows you to run the script without the need for a password. Great to use with things such as `dockd`(docking daemon)
- Run it manually with `sudo`, entering the password each time.
- Run only as the root user.

## Issues
Please submit an issue via github should you encounter any problems.

If you can improve upon this, please submit a PR!

## Usual legal garbage
I do not provide a warranty of any sort with this script.

You are the master of your destiny.

Running at maximum clocks for any amount of time could potentially damage your graphics card.

I _personally_ use the max state because my card can't really be pushed beyond it's advertised capabilities.

Please be careful.
