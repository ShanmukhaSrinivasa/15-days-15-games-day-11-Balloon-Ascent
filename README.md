15-Days-15-Games-Day-11-Balloon-Ascent

This is the eleventh game from my "15 Days 15 Games" challenge. It is a 3D side-scrolling game in the "flappy" genre, featuring a unique physics-based "hold-to-float" control mechanic.

🚀 About the Game

The player controls a balloon that automatically moves from left to right across a seamlessly looping background. By holding down a key, the player can apply a continuous upward force to the balloon to control its altitude. The player must navigate through procedurally spawned collectibles (money) and hazards (bombs). Hitting a bomb results in a game over, while collecting money increases the score.

💡 Technical Highlights

Engine: Unity (3D)

Physics-Based Floating Mechanic: The PlayerControllerX implements a "hold-to-float" system by using Rigidbody.AddForce within the Update() loop, conditional on Input.GetKey(). This creates a smooth, continuous vertical movement that contrasts with the typical impulse-based "flap" mechanic.

Component-Based and Reusable Code: The project heavily leverages a library of reusable, single-purpose scripts created during the challenge, including MoveLeftX.cs, RepeatBackgroundX.cs, and SpinObjectsX.cs. This demonstrates a modular and efficient development workflow.

Separation of Concerns: A dedicated SpawnManagerX handles all object spawning logic, keeping this responsibility separate from the GameManager, which manages the overall game state, UI, and scoring.

Polished Player Feedback: The game provides clear visual and auditory feedback for key events, utilizing ParticleSystem.Play() for firework/explosion effects and AudioSource.PlayOneShot() for sound effects upon collecting items or crashing.

▶️ Play the Game!

You can play the game in your browser on its itch.io page:
