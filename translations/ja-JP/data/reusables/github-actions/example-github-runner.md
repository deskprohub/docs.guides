### 様々なオペレーティングシステム上での実行

The starter workflow configures jobs to run on Linux, using the {% data variables.product.prodname_dotcom %}-hosted `ubuntu-latest` runners. `runs-on`キーを変更し、異なるオペレーティングシステムでジョブを実行するようにすることができます。 たとえば、{% data variables.product.prodname_dotcom %}ホストのWindowsランナーを使うことができます。

{% raw %}
```yaml
runs-on: windows-latest
```
{% endraw %}

あるいは{% data variables.product.prodname_dotcom %}ホストのmacOSランナーで実行させることもできます。

{% raw %}
```yaml
runs-on: macos-latest
```
{% endraw %}

Dockerコンテナ上でジョブを実行させたり、独自のインフラストラクチャ上で動作するセルフホストランナーを提供したりすることもできます。 詳細については、「[{% data variables.product.prodname_actions %}のワークフロー構文](/actions/automating-your-workflow-with-github-actions/workflow-syntax-for-github-actions#jobsjob_idruns-on)」を参照してください。
