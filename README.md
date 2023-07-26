# Tennis-Robot

This is a project of a tennis robot that can help people play tennis.
We'll call him "Ball boy - Deshigaoya" for now, and he can help us pick up balls, keep score, time reminders, serve tea and water, anything you'd expect to get on a non-competitive tennis court, except being your opponent, at least not right now.


## Table of Contents

1. Design
2. Hardware
3. Software
4. Future Work
5. References

## Design

The design of the robot is based on the following requirements:

1. The robot should be able to pick up balls from the ground and put them in a basket.
2. The robot should be able to keep score.
3. The robot should be able to serve tea and water.
4. The robot should be able to time reminders.
5. The robot should be able to play music.
6. The robot should be able to be communicated with via a neural language interface.

## Hardware

The hardware of the robot is based on the following requirements:

1. Nvida Jetson Orin

## Software

The software of the robot is based on the following requirements:

1. Brain

    * 参考
        * [SayCan](https://say-can.github.io/assets/palm_saycan.pdf)(2204)
        * [Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents](https://arxiv.org/pdf/2201.07207.pdf)(2201)
        * [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/pdf/2304.03442v1.pdf)(2304)
        * [VIMA: General Robot Manipulation with Multimodal Prompts](https://vimalabs.github.io/) (ICML 2023)
        
2. Control
    * 参考
        * [VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models](https://voxposer.github.io/) (2307)
3. Vision
4. Mobile
5. Manipulation
6. Interaction

### Infrastructure
1. DDS
    * 参考
        * [RustDDS](https://github.com/jhelovuo/RustDDS)
1. Robotic framework
    * 参考
        * [Dora](https://dora.carsmos.ai/)
        * [ROS2](https://docs.ros.org/en/rolling/)
1. Running LLM on bare metal
    * 参考
        * [ggml](https://github.com/ggerganov/ggml) is the library used to write [llama.cpp](https://github.com/ggerganov/llama.cpp). llama.cpp is able to run on small phone devices. [This discussion](https://github.com/ggerganov/llama.cpp/discussions/915) is also really helpful. See if we could port that library to rust.
        * [llama2.c](https://github.com/karpathy/llama2.c) is a "fullstack" train + inference solution for Llama 2 LLM, with a focus on minimalism and simplicity. llama2.c can train the Llama 2 LLM architecture from scratch in PyTorch, then export the weights to a binary file, and load that into one ~simple 500-line C file (run.c) that inferences the model.

## Future Work

Please wait for the release

## References

1. [Nvidia Jetson Orin](https://developer.nvidia.com/embedded/jetson-orin)



