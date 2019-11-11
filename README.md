# mysql-foreground
It allows you to foreground official mysql image

## Explanation

Official MySQL images does not catch CTRL + C (SIGINT) by design. So you cannot use docker with `-it --rm` to close mysqld proccess. This image fix that by using [this workaround](https://github.com/docker-library/mysql/issues/47#issuecomment-147397851).
