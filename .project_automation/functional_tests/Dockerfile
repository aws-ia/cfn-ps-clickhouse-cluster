FROM public.ecr.aws/codebuild/amazonlinux2-x86_64-standard:5.0
RUN yum install -y yum-utils \
 && yum-config-manager --add-repo https://cli.github.com/packages/rpm/gh-cli.repo  \
 && yum remove -y yum-utils \
 && yum install -y gh \
 && yum -y clean all && rm -rf /var/cache \
 && pip3 install --no-cache-dir taskcat yq \
 && gem install asciidoctor
