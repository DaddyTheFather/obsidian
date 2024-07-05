FROM ubuntu:20.04

# Install dependencies
RUN apt-get update && \
    apt-get install -y wget fuse && \
    apt-get clean

# Install Obsidian
RUN mkdir /obsidian && \
    wget https://github.com/obsidianmd/obsidian-releases/releases/download/v0.12.19/Obsidian-0.12.19.AppImage -O /obsidian/obsidian.AppImage && \
    chmod +x /obsidian/obsidian.AppImage

WORKDIR /obsidian

# Command to run Obsidian
CMD ["./obsidian.AppImage"]
