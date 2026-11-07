# Partition Size Assignment

Digital forensics assignment: calculating the size of GPT disk partitions from their first sectors, using WinHex.

## What I did
- Read the disk details (GPT, 512 bytes per sector) in WinHex
- Found each partition's sector count by subtracting its first sector from the first sector of the next partition
- Converted sectors to bytes, KB, MB and GB
- Checked the results against the Size column in the partition table

## Results
| Partition | Sectors | Size |
|-----------|---------|------|
| 1 | 204,800 | 100 MB (about 0.10 GB) |
| 2 | 32,768 | 16 MB (about 0.02 GB) |

The full write-up is in My_Assignment.docx.
