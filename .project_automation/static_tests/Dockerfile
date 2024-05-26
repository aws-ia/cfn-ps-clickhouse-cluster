FROM public.ecr.aws/codebuild/amazonlinux2-x86_64-standard:5.0
RUN git clone https://github.com/aws-quickstart/qs-cfn-lint-rules.git /tmp/qs-cfn-lint-rules \
 && cd /tmp/qs-cfn-lint-rules \
 && git checkout 2e84337d96e56ee8aea2afa761709b334c2dddaf \
 && pip3 install --no-cache-dir . \
 && pip3 install --no-cache-dir cfn-lint==0.87.3
#RUN cfn-lint -u
