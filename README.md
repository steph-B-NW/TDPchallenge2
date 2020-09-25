# CHALLENGE 2
Week 2

Task

Here is a Flask app. Your tasks is to run this application in a Docker container.
You may notice that the application uses an SQL database. This needs to be in a separate container. All secrets should be secure and not publicly available.
Flask-App - (https://gitlab.com/qacdevops/trio-task/-/tree/master)

# Stretch Goals

Create a third container that acts as a reverse proxy to the application. (NGINX)

# Submission

You should create a public Github repository that contains your Dockerfiles and a `deploy.sh` that contains all the commands you executed to run the application.
You are also expected to make a README.md file and to fill this README with information of this challenge. It should contain the following headers.
--------------------------------
# What was the challenge?
create a networked pair of containers capable of pulling data from a table and executing it with a flask app.
# How I expected the challenge to go.
I was braced for this to be particularly rough, but after refreshing myself on the topics I realised that this is just binding together the various aspects, so I was fairly confident in my ability to execute.
# What went well?
understanding the concepts of building and running the dockerfiles as containers was pleasingly simple. I had very little issue (besides some capitalisations) with the dockerfiles themselves, and getting into understanding how and why to tag each build/run was satisfying as I feel like I am beginning to understand the necessity of the structure of the commands. I actually was able to get the network to run, and accessed it on my localhost:5000 (which threw up that scary looking HTML page full of errors, but I was told to regard this as a success so that's ok) I also knew exactly how to push to a new remote origin in github, which had me worried at first but went off essentially without a hitch so I was pleased that I am getting more familiar with the basic processes.
# What didn't go as planned?
I managed to fudge the filename on entrypoint which created a big error that I wouldn't have caught if it hadn't been pointed out, so I need to be careful when defining my terms. I also didn't realise that I needed to create a network between the containers to allow them to function, though this was an odd thing to forget as the exact question of "how will this pull data from that container? It can't just do it, there's no access" ran through my mind and I never addressed it. simply, steps missed due to negligance that I shouldn't be missing.
# Possible improvements for future challenges.
I'd liked to have hit the stretch goal, but I am not too broken up as the errors I made in this taught me to be more careful with how I lay out the tasks I need to complete to hit my goals. I knew about the problem, but essentially ignored it as I made an assumption, nothing in coding and network creation is free so I need to focus on putting together a more exhaustive expected build before I start in the future, as it helps me foresee incoming problems.
