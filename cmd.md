# App Engine: Qwik Start - PHP || **GSP069**

**Command:**

```bash
curl -LO https://raw.githubusercontent.com/GoogleCloudPlatform/php-docs-samples/main/appengine/standard/helloworld/app.yaml && \
git clone https://github.com/GoogleCloudPlatform/php-docs-samples.git && \
cd php-docs-samples/appengine/standard/helloworld && \
sed -i 's/^runtime: php.*/runtime: php83/' app.yaml && \
sed -i 's/hello world!/goodbye world!/' index.php && \
gcloud app create --region=us-central1 --quiet || true && \
gcloud app deploy --quiet
