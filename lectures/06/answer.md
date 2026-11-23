# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：1つ目では、[search_materials]で2つ目では、[search_glossary]が見えているツール名であった。
- STEP 2 の [tool call]：glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：aws_aws___search_documentation({'topics': ['general'], 'search_phrase': 'Amazon S3 バージョニング 概要'})
- 気づき・疑問：awsではモデル応答回数が3回になっていた。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎
- やったこと：app/mcp_sever.pyを開き、TODOの行の下に、server.tool()(tools.get_lecture_summary)を追加した
- 結果：glossary_get_lecture_summaryが増えた,「第2回では何を学びますか」という質問で書き足したツールがよばれることを確認,pytestが通ることを確認
- 気づき・疑問：エージェント側を変えていないのに、公開するツールを決めるファイルを変更することで足したツールが使えることに驚いた。
