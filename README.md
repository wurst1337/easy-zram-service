# Easy zram service
Script to create a systemd service (unit) for creating a zram half of ram memory.

**Need / Dependencies**
- systemd
- bash
- linux
- free root disk space (equal a half of you ram memory)

**How it's work**
1) Creating a script to create zram as a half of ram
2) Creating a systemd unit to run script automaticly
3) Enable a systemd unit
4) ```swapon --show```; ```zramctl```;

---

**Possible setup**
- OS: `Arch Linux`
- Systemd: `base`
- RAM: `16GB`
- Free root disk space: `40GB`

**Result**
- Free root disk space: `40GB` - `~8GB of SwapFile` = `~32GB`
- RAM: `16GB` + `~8GB` = `16GB RAM` and `~8GB Swap`
- To check you Swap enter the command - `swapon --show`
