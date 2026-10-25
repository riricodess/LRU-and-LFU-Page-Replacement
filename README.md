# LRU-LFU-Page-Replacement

This repository contains C programs implementing the **LRU (Least Recently Used)** and **LFU (Least Frequently Used)** page replacement algorithms, based on Experiment 11 of the Operating Systems lab manual.

## Programs Included

- **LRU (Least Recently Used):** Simulates a CDN edge cache that stores three video segments. When the cache is full, it evicts the segment that has not been accessed for the longest time.
- **LFU (Least Frequently Used):** Simulates a CDN edge cache that stores three video segments. When the cache is full, it evicts the segment with the lowest access frequency. If frequencies are tied, the least recently used segment is evicted.

## Real-World Application

These algorithms are used in Content Delivery Networks (CDNs) and video streaming systems to manage cached video segments efficiently.

## Files Included

- `lru.c` – C program implementing LRU.
- `lfu.c` – C program implementing LFU.
- `LRU-output.png` – Output image for the LRU program.
- `LFU-output.png` – Output image for the LFU program.

## Requirements

- GCC compiler
- Linux terminal or Ubuntu environment

## Compilation and Execution

### LRU Program

Compile and run the LRU program using:

```bash
gcc lru.c -o lru
./lru
```

### LFU Program

Compile and run the LFU program using:

```bash
gcc lfu.c -o lfu
./lfu
```

## Conclusion

This experiment demonstrates two different cache replacement strategies. LRU replaces the least recently accessed segment, while LFU replaces the least frequently accessed segment. Both algorithms help manage limited cache capacity efficiently.
