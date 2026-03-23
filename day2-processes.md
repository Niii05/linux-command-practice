# Day 2 - Linux Processes

## Commands Learned

ps  
→ Shows processes running in current terminal  

ps aux  
→ Shows all processes running in the system  

ps aux | grep <name>  
→ Used to find a specific process  

top  
→ Shows live system processes (CPU, memory usage)  

htop  
→ Interactive and better version of top  

kill <PID>  
→ Used to stop a process  

---

## Key Concepts

Process = A running program in the system  

Examples of processes:
- bash (terminal)
- docker
- nginx  

PID (Process ID) = Unique number given to each process  

---

## Observations

- `ps` shows limited processes (current session only)  
- `ps aux` shows all system processes  
- `grep` helps filter specific processes  
- `grep` itself also appears as a process  
- `top` shows real-time system activity  
- `htop` is easier and interactive compared to top  

---

## Example Commands

ps aux | grep bash  
ps aux | grep docker  

---

## What I Understood

- System runs multiple processes at the same time  
- We can monitor and control processes  
- Process management is important for debugging servers  
