# aws-cli
A simple container with Python and the latest AWS CLI

## How to use
Running this image in a container:

```
docker run --rm -it pointw/aws-cli
```

brings you straight to a command prompt where you can run aws commands.

First run ```aws configure```, enter your access key, secret key, region, etc.

Alternately you can run with those values in environment variables:

```
docker run --rm -it -e "AWS_ACCESS_KEY_ID=AAAA" -e "AWS_SECRET_ACCESS_KEY=BBBB" -e "AWS_DEFAULT_REGION=us-east-2" pointw/aws-cli
```

(replace AAAA and BBBB with your actual access keys, of course).

You can reuse the container by dropping the ```--rm```, saving having to always run ```aws configure``` or pass the environment variables.  Or you could even build a new image based on this one with those values specified - just don't push that image anywhere public.

See also:
[AWS CLI Command Reference](http://docs.aws.amazon.com/cli/latest/reference/)
[AWS CLI Environment Variables](http://docs.aws.amazon.com/cli/latest/userguide/cli-environment.html)
