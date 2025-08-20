## ReadMe (English)
### `Summary Site Generation Prompt` ReadMe
#### 1. Overview
This prompt automatically generates an interactive website from uploaded images of sticky notes, summarizing the ideas and opinions written on them.
It is useful for visually organizing and sharing the results of brainstorming sessions and workshops.

#### 2. Key Features
* **Text Extraction and Summarization**:
   Automatically extracts text from sticky note images and summarizes the content of each note into a single, concise sentence.
* **Automatic Categorization**:
   Classifies each summarized opinion based on its context (Major Category) and intent (Type-based Category).
   * ***Major Categories (4 total)***: Lectures & Education, Research, Daily Work, Daily Life & Others.
   * ***Type-based Categories (3 total)***: Current Usage, Future Use & Ideas, Questions, Issues, & Concerns.
* **Interactive Mind Map**:
   Visualizes all opinions as a mind map centered around "Generative AI". You can pan and zoom the map with your mouse.
* **Automatic Q&A Generation**:
   The AI generates sincere and cautious answers for all items classified as "Questions, Issues, & Concerns".
* **Custom Answer Integration (PickUp Answers)**:
   Allows you to display user-provided answers for specific questions separately on the website.

#### 3. How to Use
1. Copy the entire content of the `Prompt_for_Knowledge_Sharing.txt` file.
2. Upload all the sticky note images you wish to summarize to your AI assistant's interface. (Because we generated the website using Gemini in this paper, Gemini may be prefarable.)
3. After uploading, paste the copied prompt and execute it using Gemini's Canvas feature.
4. **(Optional)** To add answers to specific questions, follow the instructions in the prompt and write your Q&A in the "PickUp Answer Format".
5.  Once the process is complete, the website will be generated as a single HTML file.

#### 4. Generated Website Specifications
* **Libraries Used**: `tailwindcss`, `d3.js` 
* **Fonts**: `Noto Sans JP`, `Inter` 
* **Page Structure**:
   * **Tab Navigation**: Tabs for "Overall View (Mind Map)" and each Major Category are placed at the top of the page.
   * **Overall View Tab**: Displays an interactive mind map rendered with D3.js.
   * **Category Tabs**: Within each category, "Usage," "Ideas," and "Concerns" are organized in a card format.The Q&A section is implemented with an accordion UI, allowing answers to be expanded and collapsed on click.

## ReadMe (日本語)
### `まとめサイト開発プロンプト` ReadMe
#### 1. 概要
このプロンプトは、アップロードされた複数の付箋の画像から、そこに書かれたアイデアや意見をまとめたインタラクティブなWebサイトを自動で生成するためのものです。
ブレーンストーミングやワークショップの結果を、視覚的に分かりやすく整理・共有するのに役立ちます。

#### 2. 主な機能
* **テキストの抽出と要約**:
    付箋の画像からテキストを自動で読み取り、1枚につき1つの簡潔な文章に要約します。
* **意見の自動分類**:
   要約された各意見を、内容の文脈（大分類）と意図（種類別分類）に基づいて自動で分類します 。
   * ***大分類 (4つ)***: 授業・教育、研究、日常業務、日常生活・その他 
   * ***種類別分類 (3つ)***: 現在の利用状況、今後の活用希望・アイデア、疑問・課題・懸念 
* **インタラクティブなマインドマップ**:
   すべての意見を「生成AI」を中心としたマインドマップとして可視化します。マウス操作で拡大・縮小や移動が可能です 。
* **Q&Aの自動生成**:
   「疑問・課題・懸念」に分類された項目に対して、AIが誠実かつ慎重な回答を生成します 。
* **カスタム回答（PickUp回答）の追加**:
   特定の質問に対して、ユーザーが用意した回答をWebサイト上に別途表示させることができます。

#### 3. 使い方
1. `まとめサイト開発プロンプト.txt` に記載されているプロンプトの全文をコピーします 。
2. AIアシスタントのインターフェースで、まとめたい付箋の画像をすべてアップロードします 。本論文ではGeminiを使用しました。
3. アップロード後、コピーしたプロンプトを貼り付けて実行します。実行時はGeminiのCanvas機能を有効にしてください。
4. **(任意)** 特定の質問への回答を追加したい場合は、プロンプトの指示に従い「PickUp回答フォーマット」にQ&Aを記述してください 。
5.  処理が完了すると、単一のHTMLファイルとしてWebサイトが生成されます。

#### 4. 生成されるWebサイトの仕様
* **使用ライブラリ**: `tailwindcss`, `d3.js` 
* **フォント**: `Noto Sans JP`, `Inter` 
* **ページ構成**:
   * ***タブナビゲーション***: ページ上部に「全体像（マインドマップ）」と各大分類ごとのタブが設置されます 。
   * ***全体像タブ***: D3.jsで描画されたインタラクティブなマインドマップが表示されます 。
   * ***カテゴリー別タブ***: 各カテゴリーごとに、「利用状況」「活用希望」「疑問・課題」などがカード形式で整理して表示されます 。Q&Aセクションは、クリックで回答が開閉するアコーディオン形式のUIで実装されます 。
