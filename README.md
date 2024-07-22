### what is it?

unlimited chat with Meta AI's Llama3 8b model.

### how does it work?

it's basically a self-hosted docker container in the cloud with llama3 available with a port open for communication(container port forwarded to server's port). the next app connects to this listening port and sends API calls.

because the project is hosted on vercel, the hobby plan just has a serverless function invocation time limit of 5s. therefore, my slow ass GPUless server struggles to generate words at pace, leading to a bad 504 bad gateway...(fixes are welcome)

### why is it super slow?

LLMs need GPUs to crank out stuff(at a reasonable speed), but the computer i'm renting doesn't have one. (sponsor? 👉👈, just kidding)
