FROM ubuntu:20.04

RUN apt-get update && \
    apt-get install -y wget fuse && \
    apt-get clean

RUN mkdir /obsidian && \
    wget https://github.com/obsidianmd/obsidian-releases/releases/download/v0.12.19/Obsidian-0.12.19.AppImage -O /obsidian/obsidian.AppImage && \
    chmod +x /obsidian/obsidian.AppImage

WORKDIR /obsidian

CMD ["./obsidian.AppImage"]
