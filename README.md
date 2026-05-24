# Hello, Captain! 🐳
 
A minimal Docker project that prints "Hello, Captain!" to the console.
 
> Project based on [roadmap.sh](https://roadmap.sh/projects/basic-dockerfile)
 
## Requirements
 
- [Docker](https://docs.docker.com/get-docker/) installed on your machine
## Project Structure
 
```
.
└── Dockerfile
```
 
## The Dockerfile
 
Create a file named `Dockerfile` in the root of the project with the following content:
 
```dockerfile
FROM alpine:latest
CMD ["echo", "Hello, Captain!"]
```
 
## Usage
 
**Build the image:**
 
```bash
docker build -t hello-captain .
```
 
**Run the container:**
 
```bash
docker run hello-captain
```
 
**Expected output:**
 
```
Hello, Captain!
```
 
## How It Works
 
| Instruction | Description |
|-------------|-------------|
| `FROM alpine:latest` | Uses the lightweight Alpine Linux image as the base |
| `CMD ["echo", "Hello, Captain!"]` | Prints the message to the console when the container starts, then exits |
