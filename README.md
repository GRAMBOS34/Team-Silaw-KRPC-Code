# _FOLLOW THE DOCS_

They should be located in `/krpc7th-simulator/docs`

I'm not going to explain how to use WSL here cus I didn't do that lmao.

# Cloning the project

Open a terminal and go into your project directory and just run

```
git clone https://github.com/GRAMBOS34/Team-Silaw-KRPC-Code.git
```

I recommend using VS Code since the git integration has a UI and is less of a pain in the ass than keeping a secret token just for you to commit something.

# Running the Simulator

Once you have successfully built the project, run `simulation.sh`

```
cd krpc7th-simulator
./simulation.sh
```

And then open a browser and open `https://localhost`

# Making Code

Based on the docs, we're limited to editing whatever is in this directory. That's why I'm unsure of whether editing those two files is allowed, especially since I couldn't even get it running.

```
/krpc7th-simulator/users/catkin_ws/src/krpc_user
```

And you may also notice that you don't have a lot of the python modules. _I THINK_ it'll be fine as they probably exist within the docker image, its just that you're kind of stuck with seeing the error squiggles if you're using a proper code editor like VS Code (hopefully)

# Commiting Code

It may be a good idea for us to have separate branches and just request a merge when needed so that we don't break everything all at once by accident.
