<div align="center">
	<br>
	<div>
		<img width="659" height="440" src="https://www.docker.com/wp-content/uploads/2023/08/logo-guide-logos-2.svg" alt="ky">
	</div>
	<br>
	<br>
  <h1>protomodule/docker:cli</h1>
  <p>
    <sup>
      Enhanced Docker CLI for usage in CI/CD pipelines
    </sup>
  </p>
	<br>
	<br>
	<br>
	<br>
	<br>
	<br>
	<br>
	<br>
</div>

> `protomodule/docker:cli` is a tiny and elegant wrapper based on the [docker:cli](https://github.com/docker-library/docker) image

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Benefits over plain `docker:cli`

- [curl](https://curl.se)
- [git](https://git-scm.com)
- [jq](https://jqlang.github.io/jq/)
- [yq](https://mikefarah.gitbook.io/yq)
- [envsubst](https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html)
- [apache2-utils](https://pkgs.alpinelinux.org/contents?name=apache2-utils&arch=x86_64&repo=main)
- [bash](https://www.gnu.org/software/bash/)

## Usage

This image has been created to run Docker based pipelines with a small set of tools commonly used in [protomodule helpers](https://github.com/protomodule/ops).

```sh
docker run --rm -it \
  protomodule/docker:cli sh -c "$(cat <<EOS
    # Your commands here ...
    docker -v
EOS
)"
```
