# Run n8n using Docker

docker run -d \
 --name n8n \
 -p 5678:5678 \
 -v D:\n8n\Yt_Automation\audio:/home/node/audio \
 -v D:\n8n\Yt_Automation\videos:/home/node/videos \
 -v D:\n8n\Yt_Automation\images:/home/node/images \
 -v D:\n8n\Yt_Automation\subtitles:/home/node/subtitles \
 -v D:\n8n\Yt_Automation\temp:/home/node/temp \
 n8nio/n8n
