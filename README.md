# ScriptHookV Template

ScriptHookV is a complicated scripting place to get started with C++. It took me hours to find create a suitable template that works when building, that I why this is here

I wanted to create something that would showcase ScriptHookV and also have the essentials to start out.

I just want to say that all credit goes to Alexander Blade for ScriptHookV and Native Menu (which where I got the Template Files)

## Downloading onto computer:

There are 2 ways that you can download the ScriptHookV Template onto your computer.

1. Going to the releases section, and downloading the latest release
2. Cloning the repository to your PC

The 1st way it easier than the 2nd way, but the 2nd way is easier if you already have a Git Console or something similar on your PC.

### INSTRUCTIONS:

#### Releases Way

1. Goto [this](https://github.com/blockba5her/ScriptHookV_Template/releases) website
2. Find the latest release (At the top)
3. Download the source code in ¨zip¨ form.
4. Extract that to your PC somewhere, and that is the template code
* You can now rename everything that you would like, and change directories and such.

#### Git Bash Way

1. Right click in the dir you want to place the template in
2. Open GitBash
3. Clone the following link `https://github.com/blockba5her/ScriptHookV_Template.git`
* Again, you can now rename everything that you would like, and change directories and such.

## Starting

Where you would start in the project is by opening the project file (the ".sln" file)
Inside the project, there is a file called "script.cpp", open that by double clicking it.
In there, there is 2 methods, one is shown as
```cpp
void ScriptMain() {
  srand(GetTickCount());
  throw main();
}
```
And the other as
```cpp
int main() {
  return 0;
}
```
All of your code would go in the `int main()` method, and please don't touch the `void ScriptMain()` method unless you know what you are doing.
Make sure to put a `while (true)` loop with a `scriptWait(0)` inside the `int main()` method or else your game will crash.

## Commons:

There will be a lot of common things that you will use in the template.
Here are a list of the most common functions
```cpp
void scriptWait(int time); // "time" in milliseconds
Ped PLAYER::PLAYER_PED_ID();
Player PLAYER::PLAYER_ID();
int std::strlen(char* string); // Length of the characters in the string input
Ped PED::CREATE_PED(int pedType, Hash modelHash, float x, float y, float z, float heading, BOOL isNetwork, BOOL p7); // Creates a ped
Vehicle VEHICLE::CREATE_VEHICLE(Hash modelHash, float x, float y, float z, float heading, BOOL isNetwork, BOOL p6); // Creates a vehicle
bool ENTITY::DOES_ENTITY_EXIST(Entity entity);
Vector3 vector = *(new Vector3()); // Creates a managed Vector3
```
Most of the above are natives, to look at more natives (because there are like 2,000 of them), look at the [NativeDB](http://www.dev-c.com/nativedb/)

## DISCLAIMERS:

I am not very good a C++ yet, I just wanted to share all of the information I had about it on my GitHub so that people like me can also start easliy.
If some things in the code are wrong, or bad, please create an issue or something like that so that I can edit my code and always become a better coder in C++.
Thank you for the understanding.
