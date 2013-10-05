SphinxでPDFファイル作成
=======================

ドキュメントの成果物として、保存したり印刷したりする用途で好まれるのがPDFです。SphinxからPDFを作成することもできます。

なお、SphinxからPDFを作るやり方にはいくつか方法があり、それぞれ一長一短があります。それぞれの環境や、使い勝手を参考に決めると良いでしょう。

.. list-table::
   :header-rows: 1
   :widths: 10 20 20

   - * 方法
     * メリット
     * デメリット
   - * rst2pdf
     * - 日本語フォント埋め込みのPDFが簡単に作れる
       - TeXがいらない
     * - rst2pdfという外部拡張を読み込む必要がある。
       - blockdiag等の外部拡張が反映されない。
   - * latex経由
     * - 見た目の綺麗なPDFが作れる
       - blockdiag等の外部拡張が反映される。
     * - TeXが必要
       - make一発では生成できない
       - Sphinx内蔵のスタイルと、日本語に適したpLaTeXの相性が良くない
     
.. toctree::
   :maxdepth: 2

   rst2pdf
   latex

.. note::

   これ以外にも、Word 2007を出力するビルダーが開発中であり、これを使うとGUIで簡単にスタイルが設定できるPDF作成環境ができる見込みです。
