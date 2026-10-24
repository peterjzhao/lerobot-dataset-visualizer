# Custom LeRobot Visualizer

A browser-based fork of Hugging Face's Apache-2.0 LeRobot Dataset Visualizer for inspecting synchronized recordings, robot motion, and user-supplied scene objects.

The current customization adds static scene composition to 3D Replay. Users can import self-contained GLB models or scene JSON, add box primitives, edit poses, and export the scene. Original robot datasets remain unchanged. Added objects are user-authored context, not measured object trajectories or physics simulation.

Use ROS REP-103 conventions for public scene coordinates: right-handed, meters, radians, X forward, Y left, Z up. The `world` frame is the scene root; `base_link` is the robot's URDF root placement, coincident with `world` by default. Standard GLB assets retain their native geometry with an explicit Y-up conversion. The renderer's historical enlargement is a display transform only.

The default entry point opens Unitree G1 Dex3 block stacking episode 0 in 3D Replay. This manufacturer-published dataset records 14 arm joints and 14 three-finger hand joints at 30 Hz; unrecorded body joints remain in the model reference pose. Dataset browsing remains available at `/?browse=1`, with humanoid examples first.
