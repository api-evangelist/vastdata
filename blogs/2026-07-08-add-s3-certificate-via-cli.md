---
title: "Add S3 Certificate via CLI"
url: "https://community.vastdata.com/t/add-s3-certificate-via-cli/2002#post_4"
date: "2026-07-08"
author: "@ram Ram Bansal"
feed_url: "https://community.vastdata.com/posts.rss"
---
Seems on the right path, is that the entire code snippet? Are you receiving an error? Here are two alternatives approaches: curl -k -u admin:123456 -X PATCH -i -F "s3_certificate=`cat cert.pem`" -F "s3_private_key=`cat key.pem`" https://vms-hostname/api/v1/clusters/1 or vastpy-cli patch clusters/1 s3_certificate="$(cat cert.pem)" s3_private_key="$(cat key.pem)"
