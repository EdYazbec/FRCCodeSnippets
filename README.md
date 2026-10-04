# FRCCodeSnippets

Learning FRC programming can be challenging. Even if you already have programming experience, the code style, vendor libraries, and framework used in FRC can take some time to learn.

**FRCCodeSnippets** is intended to bridge the gap between code generators such as [CTRE's Swerve Generator](https://v6.docs.ctr-electronics.com/en/latest/docs/tuner/tuner-swerve/index.html) and [YAMS](https://yams.yassrobotics.com/) and building entire subsystems from scratch.

The goal is to turn the process from:

> "I don't know what I'm supposed to type."

into:

> "I know what I need this motor to do, choose the appropriate code."

These snippets are not intended to cover every use case. Instead, they provide basic, safe, functional examples for configuring and controlling the motors I use most often in FRC. The current focus is on **TalonFX** and **SparkMax** motors.

The snippets currently cover:

- TalonFX / SparkMax creation
- TalonFX / SparkMax configuration
- TalonFX control
- TalonFX reading position and velocity

Supported languages:
- java

## Getting Started

Download [EdDevTools.code-snippets](EdDevTools.code-snippets) and place the file inside your project's `.vscode` folder.

## Using the Code Snippets

To use a snippet, start typing its prefix in a Java file. You do not need to type the entire prefix. VS Code's autocomplete system will find matching snippets as you type. Use the `up/down` arrows and `tab` to trigger a snippet. For example, typing `snTalonFX` will show the available TalonFX snippets.

A number of **Help** snippets are also provided to help you determine which snippet to use.

Some snippets place TODOs in the auto-completed code. Address these as you work through the generated code. The VS Code extension **Todo Tree** is a useful tool for keeping track of TODOs and making sure you don't miss any.

Some snippets also feature tab stops. Pressing `Tab` will cycle the cursor through different locations in the auto-completed code, prompting you to enter information such as motor names, CANIDs, and other configuration values.

## Snippets

| Prefix                      | Description                                           |
| --------------------------- | ----------------------------------------------------- |
| `snHelp`                    | Top-level help menu                                   |
| `snTalonFXHelp`             | TalonFX help                                          |
| `snTalonFXConfigHelp`       | TalonFX configuration help                            |
| `snTalonFXControlHelp`      | TalonFX control help                                  |
| `snSparkMaxBrushlessCreate` | Creates a SparkMax motor object for a brushless motor |
| `snSparkMaxBrushedCreate`   | Creates a SparkMax motor object for a brushed motor   |
| `snSparkMaxConfigBasic`     | Basic SparkMax motor configuration                    |
| `snSparkMaxConfigPose`      | SparkMax basic positional control configuration       |
| `snSparkMaxConfigFollower`  | SparkMax basic follower configuration                 |
| `snTalonFXCreate`           | Creates a TalonFX motor object                        |
| `snTalonFXConfigBasic`      | TalonFX basic configuration                           |
| `snTalonFXConfigPosition`   | TalonFX basic positional configuration                |
| `snTalonFXConfigVelocity`   | TalonFX basic velocity configuration                  |
| `snTalonFXConfigFollower`   | TalonFX basic follower configuration                  |
| `snTalonFXControlBasic`     | TalonFX basic spinning                                |
| `snTalonFXControlPose`      | TalonFX move-to-position request                      |
| `snTalonFXControlVel`       | TalonFX move-at-speed request                         |
| `snTalonFXGetPose`          | Gets the current TalonFX position                     |
| `snTalonFXGetVel`           | Gets the current TalonFX velocity                     |
