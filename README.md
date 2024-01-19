# 🌐 ssl_explorer

## Description
🔍 ssl_explorer is a tool designed for cybersecurity professionals and ethical hackers. It streamlines the extraction of SSL/TLS certificate information from specified URLs, crucial for target reconnaissance in security assessments and penetration testing.

Thx to Choca for this awesome tool, good job my friends

## Features
- 🔐 Extracts SSL/TLS certificate information from URLs.
- 📁 Supports processing multiple URLs via an input file.
- 🌟 Offers single URL processing.
- ⚙️ Concurrent processing with customizable thread count.
- 📊 Outputs results in a readable CSV format.

## Installation
Install ssl_explorer using `go install`:
```
GO111MODULE=on go install github.com/tucommenceapousser/ssl@latest
```

## Run on replit
[![Run on Replit](https://replit.com/badge/github/tucommenceapousser/ssl)](https://replit.com/github/tucommenceapousser/ssl)

```
chmod +x ./ssl
```

## Usage
To use ssl_explorer, specify either a single URL or provide a file containing multiple URLs.

Single URL:
```
./ssl -url=https://example.com
```

Multiple URLs from a file:
```
./ssl -input=urls.txt
```

Specify the number of concurrent threads (default is 5):
```
./ssl -input=urls.txt -threads=10
```

To save output to a file:
```
./ssl -input=urls.txt -output=results.csv
```
