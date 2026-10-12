# FOLLOW

the docs on the installation

They should be located in `/krpc7th-simulator/docs`

Should you run into some issues when building the project, I have added a `build_mods` folder where you can use the files in there to replace the respective file in the simulator directory.

# Issues I had

I've also kept the original scripts just in case. Although I don't exactly know if these are violations to the rules.

That's why if you check the folder you may see that its just the original.

## Stuck at Step 12/61 of the build

- I figured out that the PLATFORM_ARG variable was initialized in the Dockerfile but no value was assigned to it.
- I changed the bash script so it did that
- **HOWEVER**, if you're using a computer usign the ARM architecture, just use the original script it might work
- Change the `build.sh` file

## 2. Stuck at step 54/61 of the build

- I figured out that the "catkin_make" was running into issues with permissions so I explicitly changed ownership again. idk what the next touch command was for though, i just took it from gemini lmfao
- Change the `Dockerfile.krpc.base` located in `/krpc7th-simulator/docker`

## 3. It takes a long time

- Yeah it normally does but this only applies to the first build
- Just be glad you don't have to do it nearly 10 times, with each attempt taking nearly an hour, trying to solve issues

### Note

Idk how much I can attribute this to my using Arch vs to it being some oversights ("But it works on my machine" type of stuff).

# Running the Simulator

Once you have successfully built the project, run `simulation.sh`

```
cd krpc7th-simulator
./simulation.sh
```

And then open a browser and open `https://localhost`
