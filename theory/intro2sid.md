<!DOCTYPE html>

<html lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black">
    <meta name="mobile-web-app-capable" content="yes">
    <title>
        Introduction to Distributed Intelligent Agent Systems - HackMD
    </title>
    <link rel="icon" type="image/png" href="https://hackmd.io/favicon.png">
    <link rel="apple-touch-icon" href="https://hackmd.io/apple-touch-icon.png">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha256-916EbMg70RQy9LHiGkXzG8hSg9EdNy97GazNG/aiY1w=" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" integrity="sha256-eZrrJcwDc/3uDhsdt61sL2oOBY362qM3lon1gyExkL0=" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/ionicons/2.0.1/css/ionicons.min.css" integrity="sha256-3iu9jgsy9TpTwXKb7bNQzqWekRX7pPK+2OLj3R922fo=" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/octicons/3.5.0/octicons.min.css" integrity="sha256-QiWfLIsCT02Sdwkogf6YMiQlj4NE84MKkzEMkZnMGdg=" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.5.1/themes/prism.min.css" integrity="sha256-vtR0hSWRc3Tb26iuN2oZHt3KRUomwTufNIf5/4oeCyg=" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@hackmd/emojify.js@2.1.0/dist/css/basic/emojify.min.css" integrity="sha256-UOrvMOsSDSrW6szVLe8ZDZezBxh5IoIfgTwdNDgTjiU=" crossorigin="anonymous" />
    <style>
        @import url(https://fonts.googleapis.com/css?family=Roboto:300,300i,400,400i,500,500i|Source+Code+Pro:300,400,500|Source+Sans+Pro:300,300i,400,400i,600,600i|Source+Serif+Pro&subset=latin-ext);.hljs{display:block;background:#fff;padding:.5em;color:#333;overflow-x:auto}.hljs-comment,.hljs-meta{color:#969896}.hljs-emphasis,.hljs-quote,.hljs-string,.hljs-strong,.hljs-template-variable,.hljs-variable{color:#df5000}.hljs-keyword,.hljs-selector-tag,.hljs-type{color:#a71d5d}.hljs-attribute,.hljs-bullet,.hljs-literal,.hljs-number,.hljs-symbol{color:#0086b3}.hljs-built_in,.hljs-builtin-name{color:#005cc5}.hljs-name,.hljs-section{color:#63a35c}.hljs-tag{color:#333}.hljs-attr,.hljs-selector-attr,.hljs-selector-class,.hljs-selector-id,.hljs-selector-pseudo,.hljs-title{color:#795da3}.hljs-addition{color:#55a532;background-color:#eaffea}.hljs-deletion{color:#bd2c00;background-color:#ffecec}.hljs-link{text-decoration:underline}.markdown-body{font-size:16px;line-height:1.5;word-wrap:break-word}.markdown-body:after,.markdown-body:before{display:table;content:""}.markdown-body:after{clear:both}.markdown-body>:first-child{margin-top:0!important}.markdown-body>:last-child{margin-bottom:0!important}.markdown-body a:not([href]){color:inherit;text-decoration:none}.markdown-body .absent{color:#c00}.markdown-body .anchor{float:left;padding-right:4px;margin-left:-20px;line-height:1}.markdown-body .anchor:focus{outline:none}.markdown-body blockquote,.markdown-body dl,.markdown-body ol,.markdown-body p,.markdown-body pre,.markdown-body table,.markdown-body ul{margin-top:0;margin-bottom:16px}.markdown-body hr{height:.25em;padding:0;margin:24px 0;background-color:#e7e7e7;border:0}.markdown-body blockquote{font-size:16px;padding:0 1em;color:#777;border-left:.25em solid #ddd}.markdown-body blockquote>:first-child{margin-top:0}.markdown-body blockquote>:last-child{margin-bottom:0}.markdown-body kbd,.popover kbd{display:inline-block;padding:3px 5px;font-size:11px;line-height:10px;color:#555;vertical-align:middle;background-color:#fcfcfc;border:1px solid #ccc;border-bottom-color:#bbb;border-radius:3px;box-shadow:inset 0 -1px 0 #bbb}.markdown-body .loweralpha{list-style-type:lower-alpha}.markdown-body h1,.markdown-body h2,.markdown-body h3,.markdown-body h4,.markdown-body h5,.markdown-body h6{margin-top:24px;margin-bottom:16px;font-weight:600;line-height:1.25}.markdown-body h1 .octicon-link,.markdown-body h2 .octicon-link,.markdown-body h3 .octicon-link,.markdown-body h4 .octicon-link,.markdown-body h5 .octicon-link,.markdown-body h6 .octicon-link{color:#000;vertical-align:middle;visibility:hidden}.markdown-body h1:hover .anchor,.markdown-body h2:hover .anchor,.markdown-body h3:hover .anchor,.markdown-body h4:hover .anchor,.markdown-body h5:hover .anchor,.markdown-body h6:hover .anchor{text-decoration:none}.markdown-body h1:hover .anchor .octicon-link,.markdown-body h2:hover .anchor .octicon-link,.markdown-body h3:hover .anchor .octicon-link,.markdown-body h4:hover .anchor .octicon-link,.markdown-body h5:hover .anchor .octicon-link,.markdown-body h6:hover .anchor .octicon-link{visibility:visible}.markdown-body h1 code,.markdown-body h1 tt,.markdown-body h2 code,.markdown-body h2 tt,.markdown-body h3 code,.markdown-body h3 tt,.markdown-body h4 code,.markdown-body h4 tt,.markdown-body h5 code,.markdown-body h5 tt,.markdown-body h6 code,.markdown-body h6 tt{font-size:inherit}.markdown-body h1{font-size:2em}.markdown-body h1,.markdown-body h2{padding-bottom:.3em;border-bottom:1px solid #eee}.markdown-body h2{font-size:1.5em}.markdown-body h3{font-size:1.25em}.markdown-body h4{font-size:1em}.markdown-body h5{font-size:.875em}.markdown-body h6{font-size:.85em;color:#777}.markdown-body ol,.markdown-body ul{padding-left:2em}.markdown-body ol.no-list,.markdown-body ul.no-list{padding:0;list-style-type:none}.markdown-body ol ol,.markdown-body ol ul,.markdown-body ul ol,.markdown-body ul ul{margin-top:0;margin-bottom:0}.markdown-body li>p{margin-top:16px}.markdown-body li+li{padding-top:.25em}.markdown-body dl{padding:0}.markdown-body dl dt{padding:0;margin-top:16px;font-size:1em;font-style:italic;font-weight:700}.markdown-body dl dd{padding:0 16px;margin-bottom:16px}.markdown-body table{display:block;width:100%;overflow:auto;word-break:normal;word-break:keep-all}.markdown-body table th{font-weight:700}.markdown-body table td,.markdown-body table th{padding:6px 13px;border:1px solid #ddd}.markdown-body table tr{background-color:#fff;border-top:1px solid #ccc}.markdown-body table tr:nth-child(2n){background-color:#f8f8f8}.markdown-body img{max-width:100%;box-sizing:content-box;background-color:#fff}.markdown-body img[align=right]{padding-left:20px}.markdown-body img[align=left]{padding-right:20px}.markdown-body .emoji{max-width:none;vertical-align:text-top;background-color:transparent}.markdown-body span.frame{display:block;overflow:hidden}.markdown-body span.frame>span{display:block;float:left;width:auto;padding:7px;margin:13px 0 0;overflow:hidden;border:1px solid #ddd}.markdown-body span.frame span img{display:block;float:left}.markdown-body span.frame span span{display:block;padding:5px 0 0;clear:both;color:#333}.markdown-body span.align-center{display:block;overflow:hidden;clear:both}.markdown-body span.align-center>span{display:block;margin:13px auto 0;overflow:hidden;text-align:center}.markdown-body span.align-center span img{margin:0 auto;text-align:center}.markdown-body span.align-right{display:block;overflow:hidden;clear:both}.markdown-body span.align-right>span{display:block;margin:13px 0 0;overflow:hidden;text-align:right}.markdown-body span.align-right span img{margin:0;text-align:right}.markdown-body span.float-left{display:block;float:left;margin-right:13px;overflow:hidden}.markdown-body span.float-left span{margin:13px 0 0}.markdown-body span.float-right{display:block;float:right;margin-left:13px;overflow:hidden}.markdown-body span.float-right>span{display:block;margin:13px auto 0;overflow:hidden;text-align:right}.markdown-body code,.markdown-body tt{padding:0;padding-top:.2em;padding-bottom:.2em;margin:0;font-size:85%;background-color:rgba(0,0,0,.04);border-radius:3px}.markdown-body code:after,.markdown-body code:before,.markdown-body tt:after,.markdown-body tt:before{letter-spacing:-.2em;content:"\00a0"}.markdown-body code br,.markdown-body tt br{display:none}.markdown-body del code{text-decoration:inherit}.markdown-body pre{word-wrap:normal}.markdown-body pre>code{padding:0;margin:0;font-size:100%;word-break:normal;white-space:pre;background:transparent;border:0}.markdown-body .highlight{margin-bottom:16px}.markdown-body .highlight pre{margin-bottom:0;word-break:normal}.markdown-body .highlight pre,.markdown-body pre{padding:16px;overflow:auto;font-size:85%;line-height:1.45;background-color:#f7f7f7;border-radius:3px}.markdown-body pre code,.markdown-body pre tt{display:inline;max-width:auto;padding:0;margin:0;overflow:visible;line-height:inherit;word-wrap:normal;background-color:transparent;border:0}.markdown-body pre code:after,.markdown-body pre code:before,.markdown-body pre tt:after,.markdown-body pre tt:before{content:normal}.markdown-body .csv-data td,.markdown-body .csv-data th{padding:5px;overflow:hidden;font-size:12px;line-height:1;text-align:left;white-space:nowrap}.markdown-body .csv-data .blob-line-num{padding:10px 8px 9px;text-align:right;background:#fff;border:0}.markdown-body .csv-data tr{border-top:0}.markdown-body .csv-data th{font-weight:700;background:#f8f8f8;border-top:0}.news .alert .markdown-body blockquote{padding:0 0 0 40px;border:0 none}.activity-tab .news .alert .commits,.activity-tab .news .markdown-body blockquote{padding-left:0}.task-list-item{list-style-type:none}.task-list-item label{font-weight:400}.task-list-item.enabled label{cursor:pointer}.task-list-item+.task-list-item{margin-top:3px}.task-list-item-checkbox{float:left;margin:.31em 0 .2em -1.3em!important;vertical-align:middle;cursor:default!important}.markdown-body{padding-top:40px;padding-bottom:40px;max-width:758px;overflow:visible!important;position:relative}.markdown-body .emoji{vertical-align:top}.markdown-body pre{border:inherit!important}.markdown-body code{color:inherit!important}.markdown-body pre code .wrapper{display:-moz-inline-flex;display:-ms-inline-flex;display:-o-inline-flex;display:inline-flex}.markdown-body pre code .gutter{float:left;overflow:hidden;-webkit-user-select:none;user-select:none}.markdown-body pre code .gutter.linenumber{text-align:right;position:relative;display:inline-block;cursor:default;z-index:4;padding:0 8px 0 0;min-width:20px;box-sizing:content-box;color:#afafaf!important;border-right:3px solid #6ce26c!important}.markdown-body pre code .gutter.linenumber>span:before{content:attr(data-linenumber)}.markdown-body pre code .code{float:left;margin:0 0 0 16px}.markdown-body .gist .line-numbers{border-left:none;border-top:none;border-bottom:none}.markdown-body .gist .line-data{border:none}.markdown-body .gist table{border-spacing:0;border-collapse:inherit!important}.markdown-body code[data-gist-id]{background:none;padding:0}.markdown-body code[data-gist-id]:after,.markdown-body code[data-gist-id]:before{content:""}.markdown-body code[data-gist-id] .blob-num{border:unset}.markdown-body code[data-gist-id] table{overflow:unset;margin-bottom:unset}.markdown-body code[data-gist-id] table tr{background:unset}.markdown-body[dir=rtl] pre{direction:ltr}.markdown-body[dir=rtl] code{direction:ltr;unicode-bidi:embed}.markdown-body .alert>p:last-child{margin-bottom:0}.markdown-body pre.abc,.markdown-body pre.flow-chart,.markdown-body pre.graphviz,.markdown-body pre.mermaid,.markdown-body pre.sequence-diagram,.markdown-body pre.vega{text-align:center;background-color:inherit;border-radius:0;white-space:inherit;overflow:visible}.markdown-body pre.abc>code,.markdown-body pre.flow-chart>code,.markdown-body pre.graphviz>code,.markdown-body pre.mermaid>code,.markdown-body pre.sequence-diagram>code,.markdown-body pre.vega>code{text-align:left}.markdown-body pre.abc>svg,.markdown-body pre.flow-chart>svg,.markdown-body pre.graphviz>svg,.markdown-body pre.mermaid>svg,.markdown-body pre.sequence-diagram>svg,.markdown-body pre.vega>svg{max-width:100%;height:100%}.markdown-body pre>code.wrap{white-space:pre-wrap;white-space:-moz-pre-wrap;white-space:-pre-wrap;white-space:-o-pre-wrap;word-wrap:break-word}.markdown-body .alert>p:last-child,.markdown-body .alert>ul:last-child{margin-bottom:0}.markdown-body summary{display:list-item}.markdown-body summary:focus{outline:none}.markdown-body details summary{cursor:pointer}.markdown-body details:not([open])>:not(summary){display:none}.markdown-body figure{margin:1em 40px}.markdown-body .mark,.markdown-body mark{background-color:#fff1a7}.vimeo,.youtube{cursor:pointer;display:table;text-align:center;background-position:50%;background-repeat:no-repeat;background-size:contain;background-color:#000;overflow:hidden}.vimeo,.youtube{position:relative;width:100%}.youtube{padding-bottom:56.25%}.vimeo img{width:100%;object-fit:contain;z-index:0}.youtube img{object-fit:cover;z-index:0}.vimeo iframe,.youtube iframe,.youtube img{width:100%;height:100%;position:absolute;top:0;left:0}.vimeo iframe,.youtube iframe{vertical-align:middle;z-index:1}.vimeo .icon,.youtube .icon{position:absolute;height:auto;width:auto;top:50%;left:50%;transform:translate(-50%,-50%);color:#fff;opacity:.3;transition:opacity .2s;z-index:0}.vimeo:hover .icon,.youtube:hover .icon{opacity:.6;transition:opacity .2s}.slideshare .inner,.speakerdeck .inner{position:relative;width:100%}.slideshare .inner iframe,.speakerdeck .inner iframe{position:absolute;top:0;bottom:0;left:0;right:0;width:100%;height:100%}.figma{display:table;position:relative;width:100%;padding-bottom:56.25%}.figma iframe{position:absolute;top:0;bottom:0;left:0;right:0;width:100%;height:100%;border:1px solid #eee}.markmap-container{height:300px}.markmap-container>svg{width:100%;height:100%}.MJX_Assistive_MathML{display:none}#MathJax_Message{z-index:1000!important}.ui-infobar{position:relative;z-index:2;max-width:760px;margin:25px auto -25px;color:#777}.toc .invisable-node{list-style-type:none}.ui-toc{position:fixed;bottom:20px;z-index:998}.ui-toc.both-mode{margin-left:8px}.ui-toc.both-mode .ui-toc-label{height:40px;padding:10px 4px;border-top-left-radius:0;border-bottom-left-radius:0}.ui-toc-label{background-color:#e6e6e6;border:none;color:#868686;transition:opacity .2s}.ui-toc .open .ui-toc-label{opacity:1;color:#fff;transition:opacity .2s}.ui-toc-label:focus{opacity:.3;background-color:#ccc;color:#000}.ui-toc-label:hover{opacity:1;background-color:#ccc;transition:opacity .2s}.ui-toc-dropdown{margin-top:20px;margin-bottom:20px;padding-left:10px;padding-right:10px;max-width:45vw;width:25vw;max-height:70vh;overflow:auto;text-align:inherit}.ui-toc-dropdown>.toc{max-height:calc(70vh - 100px);overflow:auto}.ui-toc-dropdown[dir=rtl] .nav{padding-right:0;letter-spacing:.0029em}.ui-toc-dropdown a{overflow:hidden;text-overflow:ellipsis;white-space:pre}.ui-toc-dropdown .nav>li>a{display:block;padding:4px 20px;font-size:13px;font-weight:500;color:#767676}.ui-toc-dropdown .nav>li:first-child:last-child>ul,.ui-toc-dropdown .toc.expand ul{display:block}.ui-toc-dropdown .nav>li>a:focus,.ui-toc-dropdown .nav>li>a:hover{padding-left:19px;color:#000;text-decoration:none;background-color:transparent;border-left:1px solid #000}.ui-toc-dropdown[dir=rtl] .nav>li>a:focus,.ui-toc-dropdown[dir=rtl] .nav>li>a:hover{padding-right:19px;border-left:none;border-right:1px solid #000}.ui-toc-dropdown .nav>.active:focus>a,.ui-toc-dropdown .nav>.active:hover>a,.ui-toc-dropdown .nav>.active>a{padding-left:18px;font-weight:700;color:#000;background-color:transparent;border-left:2px solid #000}.ui-toc-dropdown[dir=rtl] .nav>.active:focus>a,.ui-toc-dropdown[dir=rtl] .nav>.active:hover>a,.ui-toc-dropdown[dir=rtl] .nav>.active>a{padding-right:18px;border-left:none;border-right:2px solid #000}.ui-toc-dropdown .nav .nav{display:none;padding-bottom:10px}.ui-toc-dropdown .nav>.active>ul{display:block}.ui-toc-dropdown .nav .nav>li>a{padding-top:1px;padding-bottom:1px;padding-left:30px;font-size:12px;font-weight:400}.ui-toc-dropdown[dir=rtl] .nav .nav>li>a{padding-right:30px}.ui-toc-dropdown .nav .nav>li>ul>li>a{padding-top:1px;padding-bottom:1px;padding-left:40px;font-size:12px;font-weight:400}.ui-toc-dropdown[dir=rtl] .nav .nav>li>ul>li>a{padding-right:40px}.ui-toc-dropdown .nav .nav>li>a:focus,.ui-toc-dropdown .nav .nav>li>a:hover{padding-left:29px}.ui-toc-dropdown[dir=rtl] .nav .nav>li>a:focus,.ui-toc-dropdown[dir=rtl] .nav .nav>li>a:hover{padding-right:29px}.ui-toc-dropdown .nav .nav>li>ul>li>a:focus,.ui-toc-dropdown .nav .nav>li>ul>li>a:hover{padding-left:39px}.ui-toc-dropdown[dir=rtl] .nav .nav>li>ul>li>a:focus,.ui-toc-dropdown[dir=rtl] .nav .nav>li>ul>li>a:hover{padding-right:39px}.ui-toc-dropdown .nav .nav>.active:focus>a,.ui-toc-dropdown .nav .nav>.active:hover>a,.ui-toc-dropdown .nav .nav>.active>a{padding-left:28px;font-weight:500}.ui-toc-dropdown[dir=rtl] .nav .nav>.active:focus>a,.ui-toc-dropdown[dir=rtl] .nav .nav>.active:hover>a,.ui-toc-dropdown[dir=rtl] .nav .nav>.active>a{padding-right:28px}.ui-toc-dropdown .nav .nav>.active>.nav>.active:focus>a,.ui-toc-dropdown .nav .nav>.active>.nav>.active:hover>a,.ui-toc-dropdown .nav .nav>.active>.nav>.active>a{padding-left:38px;font-weight:500}.ui-toc-dropdown[dir=rtl] .nav .nav>.active>.nav>.active:focus>a,.ui-toc-dropdown[dir=rtl] .nav .nav>.active>.nav>.active:hover>a,.ui-toc-dropdown[dir=rtl] .nav .nav>.active>.nav>.active>a{padding-right:38px}.markdown-body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,sans-serif}html[lang^=ja] .markdown-body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,Hiragino Kaku Gothic Pro,ヒラギノ角ゴ Pro W3,Osaka,Meiryo,メイリオ,MS Gothic,ＭＳ\ ゴシック,sans-serif}html[lang=zh-tw] .markdown-body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,PingFang TC,Microsoft JhengHei,微軟正黑,sans-serif}html[lang=zh-cn] .markdown-body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,PingFang SC,Microsoft YaHei,微软雅黑,sans-serif}html .markdown-body[lang^=ja]{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,Hiragino Kaku Gothic Pro,ヒラギノ角ゴ Pro W3,Osaka,Meiryo,メイリオ,MS Gothic,ＭＳ\ ゴシック,sans-serif}html .markdown-body[lang=zh-tw]{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,PingFang TC,Microsoft JhengHei,微軟正黑,sans-serif}html .markdown-body[lang=zh-cn]{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica Neue,Helvetica,Roboto,Arial,PingFang SC,Microsoft YaHei,微软雅黑,sans-serif}html[lang^=ja] .ui-toc-dropdown{font-family:Source Sans Pro,Helvetica,Arial,Meiryo UI,MS PGothic,ＭＳ\ Ｐゴシック,sans-serif}html[lang=zh-tw] .ui-toc-dropdown{font-family:Source Sans Pro,Helvetica,Arial,Microsoft JhengHei UI,微軟正黑UI,sans-serif}html[lang=zh-cn] .ui-toc-dropdown{font-family:Source Sans Pro,Helvetica,Arial,Microsoft YaHei UI,微软雅黑UI,sans-serif}html .ui-toc-dropdown[lang^=ja]{font-family:Source Sans Pro,Helvetica,Arial,Meiryo UI,MS PGothic,ＭＳ\ Ｐゴシック,sans-serif}html .ui-toc-dropdown[lang=zh-tw]{font-family:Source Sans Pro,Helvetica,Arial,Microsoft JhengHei UI,微軟正黑UI,sans-serif}html .ui-toc-dropdown[lang=zh-cn]{font-family:Source Sans Pro,Helvetica,Arial,Microsoft YaHei UI,微软雅黑UI,sans-serif}.ui-affix-toc{position:fixed;top:0;max-width:15vw;max-height:70vh;overflow:auto}.back-to-top,.expand-toggle,.go-to-bottom{display:block;padding:4px 10px;margin-top:10px;margin-left:10px;font-size:12px;font-weight:500;color:#999}.back-to-top:focus,.back-to-top:hover,.expand-toggle:focus,.expand-toggle:hover,.go-to-bottom:focus,.go-to-bottom:hover{color:#563d7c;text-decoration:none}.back-to-top,.go-to-bottom{margin-top:0}.ui-user-icon{width:20px;height:20px;display:block;border-radius:50%;margin-top:2px;margin-bottom:2px;margin-right:5px;background-position:50%;background-repeat:no-repeat;background-size:cover}.ui-user-icon.small{width:18px;height:18px;display:inline-block;vertical-align:middle;margin:0 0 .2em}.ui-infobar>small>span{line-height:22px}.ui-infobar>small .dropdown{display:inline-block}.ui-infobar>small .dropdown a:focus,.ui-infobar>small .dropdown a:hover{text-decoration:none}.ui-more-info{color:#888;cursor:pointer;vertical-align:middle}.ui-more-info .fa{font-size:16px}.ui-connectedGithub,.ui-published-note{color:#888}.ui-connectedGithub{line-height:23px;white-space:nowrap}.ui-connectedGithub a.file-path{color:#888;text-decoration:none;padding-left:22px}.ui-connectedGithub a.file-path:active,.ui-connectedGithub a.file-path:hover{color:#888;text-decoration:underline}.ui-connectedGithub .fa{font-size:20px}.ui-published-note .fa{font-size:20px;vertical-align:top}.unselectable{-webkit-user-select:none;-o-user-select:none;user-select:none}.selectable{-webkit-user-select:text;-o-user-select:text;user-select:text}@media print{blockquote,div,img,pre,table{page-break-inside:avoid!important}a[href]:after{font-size:12px!important}}.markdown-body.slides{position:relative;z-index:1;color:#222}.markdown-body.slides:before{content:"";display:block;position:absolute;top:0;left:0;right:0;bottom:0;z-index:-1;background-color:currentColor;box-shadow:0 0 0 50vw}.markdown-body.slides section[data-markdown]{position:relative;margin-bottom:1.5em;background-color:#fff;text-align:center}.markdown-body.slides section[data-markdown] code{text-align:left}.markdown-body.slides section[data-markdown]:before{content:"";display:block;padding-bottom:56.23%}.markdown-body.slides section[data-markdown]>div:first-child{position:absolute;top:50%;left:1em;right:1em;transform:translateY(-50%);max-height:100%;overflow:hidden}.markdown-body.slides section[data-markdown]>ul{display:inline-block}.markdown-body.slides>section>section+section:after{content:"";position:absolute;top:-1.5em;right:1em;height:1.5em;border:3px solid #777}.site-ui-font{font-family:Source Sans Pro,Helvetica,Arial,sans-serif}html[lang^=ja] .site-ui-font{font-family:Source Sans Pro,Helvetica,Arial,Hiragino Kaku Gothic Pro,ヒラギノ角ゴ Pro W3,Osaka,Meiryo,メイリオ,MS Gothic,ＭＳ\ ゴシック,sans-serif}html[lang=zh-tw] .site-ui-font{font-family:Source Sans Pro,Helvetica,Arial,PingFang TC,Microsoft JhengHei,微軟正黑,sans-serif}html[lang=zh-cn] .site-ui-font{font-family:Source Sans Pro,Helvetica,Arial,PingFang SC,Microsoft YaHei,微软雅黑,sans-serif}body{font-smoothing:subpixel-antialiased!important;-webkit-font-smoothing:subpixel-antialiased!important;-moz-osx-font-smoothing:auto!important;text-shadow:0 0 1em transparent,1px 1px 1.2px rgba(0,0,0,.004);-webkit-overflow-scrolling:touch;letter-spacing:.025em;font-family:Source Sans Pro,Helvetica,Arial,sans-serif}html[lang^=ja] body{font-family:Source Sans Pro,Helvetica,Arial,Hiragino Kaku Gothic Pro,ヒラギノ角ゴ Pro W3,Osaka,Meiryo,メイリオ,MS Gothic,ＭＳ\ ゴシック,sans-serif}html[lang=zh-tw] body{font-family:Source Sans Pro,Helvetica,Arial,PingFang TC,Microsoft JhengHei,微軟正黑,sans-serif}html[lang=zh-cn] body{font-family:Source Sans Pro,Helvetica,Arial,PingFang SC,Microsoft YaHei,微软雅黑,sans-serif}abbr[title]{border-bottom:none;text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}abbr[data-original-title],abbr[title]{cursor:help}body.modal-open{overflow-y:auto;padding-right:0!important}
    </style>
    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
    	<script src="https://cdnjs.cloudflare.com/ajax/libs/html5shiv/3.7.3/html5shiv.min.js" integrity="sha256-3Jy/GbSLrg0o9y5Z5n1uw0qxZECH7C6OQpVBgNFYa0g=" crossorigin="anonymous"></script>
    	<script src="https://cdnjs.cloudflare.com/ajax/libs/respond.js/1.4.2/respond.min.js" integrity="sha256-g6iAfvZp+nDQ2TdTR/VVKJf3bGro4ub5fvWSWVRi2NE=" crossorigin="anonymous"></script>
		<script src="https://cdnjs.cloudflare.com/ajax/libs/es5-shim/4.5.9/es5-shim.min.js" integrity="sha256-8E4Is26QH0bD52WoQpcB+R/tcWQtpzlCojrybUd7Mxo=" crossorigin="anonymous"></script>
    <![endif]-->
</head>

<body>
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Introduction-to-Distributed-Intelligent-Agent-Systems" data-id="Introduction-to-Distributed-Intelligent-Agent-Systems"><a class="anchor hidden-xs" href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction-to-Distributed-Intelligent-Agent-Systems"><span class="octicon octicon-link"></span></a><span>Introduction to Distributed Intelligent Agent Systems</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction to Distributed Intelligent Agent Systems">Introduction to Distributed Intelligent Agent Systems</a><ul>
<li><a href="#Artificial-Intelligence" title="Artificial Intelligence">Artificial Intelligence</a></li>
<li><a href="#Cognitive-Architectures-I" title="Cognitive Architectures I">Cognitive Architectures I</a></li>
<li><a href="#Intelligent-Agent" title="Intelligent Agent">Intelligent Agent</a></li>
<li><a href="#Cognitive-AI-Paradigms" title="Cognitive AI Paradigms">Cognitive AI Paradigms</a></li>
<li><a href="#Cognitive-AI-Fundations" title="Cognitive AI Fundations">Cognitive AI Fundations</a><ul>
<li><a href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George Herbert Mead (1863-1931) Mind, Self, and Society">George Herbert Mead (1863-1931) Mind, Self, and Society</a></li>
</ul>
</li>
<li><a href="#MIND" title="MIND">MIND</a><ul>
<li><a href="#Analogy-An-ants-society" title="Analogy: An ants society">Analogy: An ants society</a></li>
<li><a href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)">Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</a></li>
<li><a href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin Minsky, The Society of Mind">Marvin Minsky, The Society of Mind</a></li>
</ul>
</li>
<li><a href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which Kind of Cognitive Architectures are we Looking for?">Which Kind of Cognitive Architectures are we Looking for?</a></li>
<li><a href="#Nature-of-the-Brain" title="Nature of the Brain">Nature of the Brain</a></li>
<li><a href="#Architectures-for-Reactive-Systems" title="Architectures for Reactive Systems">Architectures for Reactive Systems</a></li>
<li><a href="#Cognitive-Architectures-II" title="Cognitive Architectures II">Cognitive Architectures II</a><ul>
<li><a href="#Parameters" title="Parameters">Parameters</a></li>
<li><a href="#Open-issues" title="Open issues">Open issues</a></li>
<li><a href="#Functional-aspects" title="Functional aspects">Functional aspects</a></li>
</ul>
</li>
<li><a href="#Rational-Decisions" title="Rational Decisions">Rational Decisions</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Artificial-Intelligence" data-id="Artificial-Intelligence"><a class="anchor hidden-xs" href="#Artificial-Intelligence" title="Artificial-Intelligence"><span class="octicon octicon-link"></span></a><span>Artificial Intelligence</span></h2><ul>
<li>
<p><span>Too many definitions:</span></p>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>The theory and development of computer systems able to perform tasks normally requiring human intelligence, such as visual perception, speech recognition, decision-making, and translation between languages. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>Artificial intelligence is the ability of a digital computer or computer-controlled robot to perform tasks commonly associated with intelligent beings.</span><br><br><span>The term is frequently applied to the project of developing systems endowed with the intellectual processes characteristic of humans, such as the ability to reason, discover meaning, generalize, or learn from past experience. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>“Artificial intelligence (AI) refers to systems that display intelligent behaviour by analysing their environment and taking actions – with some degree of autonomy – to achieve specific goals." </span><em><span>-European Commission’s Communication on AI</span></em><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>Artificial intelligence (AI) systems are software (and possibly also hardware) systems designed by humans that, given a complex goal, </span><strong><span>act in the physical or digital dimension by perceiving their environment through data acquisition</span></strong><span>, interpreting the collected structured or unstructured data, reasoning on the knowledge, or processing the information, derived from this data and </span><strong><span>deciding the best action(s) to take to achieve the given goal.</span></strong><span> AI systems can either use </span><strong><span>symbolic rules or learn a numeric model</span></strong><span>, and they can also adapt their behaviour by analysing how the environment is affected by their previous actions. </span><em><span>-(HLEG-AI)</span></em><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
</li>
</ul><hr><h2 id="Cognitive-Architectures-I" data-id="Cognitive-Architectures-I"><a class="anchor hidden-xs" href="#Cognitive-Architectures-I" title="Cognitive-Architectures-I"><span class="octicon octicon-link"></span></a><span>Cognitive Architectures I</span></h2><ul>
<li><span>In this course we aim to have a </span><strong><span>holistic view</span></strong><span> of Artificial Intelligence: its methods, techniques, and how to combine them into intelligent systems.</span></li>
<li><span>But… what is an </span><strong><span>intelligent system</span></strong><span>?</span>
<ul>
<li><span>One way to characterize the behaviour we </span><strong><span>think</span></strong><span> as </span><em><strong><span>intelligence</span></strong></em><span> is through the study of the architectures providing such behaviour.</span></li>
</ul>
</li>
<li><span>We call </span><u><strong><span>Cognitive Architectures</span></strong></u><span> the ones that use </span><strong><span>symbols</span></strong><span> to represent the environment.</span>
<ul>
<li><u><span>Architectures</span></u><span> are described by the description of their foundations and the methods used to achieve an </span><em><strong><span>intelligent behaviour</span></strong></em><span>.</span></li>
<li><span>Cognitive architectures are based on computational entities, but this does not imply that intelligence should come always from the computer.</span></li>
<li><span>A metaphor typically used in Cognitive Architectures to cover both human and machine intelligence is the one of the </span><em><strong><span>intelligent agent</span></strong></em><span>.</span></li>
</ul>
</li>
</ul><hr><h2 id="Intelligent-Agent" data-id="Intelligent-Agent"><a class="anchor hidden-xs" href="#Intelligent-Agent" title="Intelligent-Agent"><span class="octicon octicon-link"></span></a><span>Intelligent Agent</span></h2><ul>
<li><u><span>An agent is a computer system capable of autonomous action in some environment in order to meet its design objectives.</span></u></li>
<li><span>An agent should be able to perceive and act in the environment.</span></li>
<li><span>Usually the environment is </span><em><strong><span>complex</span></strong></em><span> and </span><em><strong><span>dynamic</span></strong></em><span>, and agents should interact with it in real time.</span></li>
</ul><p><img src="https://i.imgur.com/P7WLLdh.png" alt="" loading="lazy"></p><hr><h2 id="Cognitive-AI-Paradigms" data-id="Cognitive-AI-Paradigms"><a class="anchor hidden-xs" href="#Cognitive-AI-Paradigms" title="Cognitive-AI-Paradigms"><span class="octicon octicon-link"></span></a><span>Cognitive AI Paradigms</span></h2><ul>
<li><span>In AI, paradigmas can be characterized by the metaphor used to model intelligence:</span>
<ul>
<li><span>Logics</span></li>
<li><span>Search in a State Space</span></li>
<li><span>Knowledge-Based (rules, patterns, experiences)</span></li>
<li><span>Evolutionary</span></li>
<li><span>Social</span></li>
</ul>
</li>
</ul><hr><h2 id="Cognitive-AI-Fundations" data-id="Cognitive-AI-Fundations"><a class="anchor hidden-xs" href="#Cognitive-AI-Fundations" title="Cognitive-AI-Fundations"><span class="octicon octicon-link"></span></a><span>Cognitive AI Fundations</span></h2><ul>
<li><span>PHILOSOPHY</span>
<ul>
<li><span>Can rules be used to extract valid conclusions? How mind emerges from the physical brain? Where does Knowledge come from? How can Knowledge lead to action?</span></li>
</ul>
</li>
<li><span>MATHEMATICS/LOGICS</span>
<ul>
<li><span>Which are the formal rules to extract valid conclusions? Which things are computable? How to reason with Knowledge that is uncertain and/or vague and/or incomplete?</span></li>
</ul>
</li>
<li><span>NEUROSCIENCES</span>
<ul>
<li><span>How is information processed by the brain?</span></li>
</ul>
</li>
<li><span>PSICOLOGY</span>
<ul>
<li><span>How do animals and humans think and act?</span></li>
</ul>
</li>
<li><span>SOCIOLOGY/ETOLOGY/ECONOMICS</span>
<ul>
<li><span>How collective (social/organizational) behaviour can be generated from individual (animal/human) behaviour?</span></li>
</ul>
</li>
<li><span>CONTROL THEORY</span>
<ul>
<li><span>How can self-controlled artifacts behave/act?</span></li>
</ul>
</li>
</ul><h3 id="George-Herbert-Mead-1863-1931-Mind-Self-and-Society" data-id="George-Herbert-Mead-1863-1931-Mind-Self-and-Society"><a class="anchor hidden-xs" href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George-Herbert-Mead-1863-1931-Mind-Self-and-Society"><span class="octicon octicon-link"></span></a><span>George Herbert Mead (1863-1931) Mind, Self, and Society</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The self is an object to itself.</span></li>
<li><span>The self is a social structure.</span></li>
<li><span>Self arises from social experience.</span></li>
<li><span>Self arises from language and interaction with others.</span></li>
<li><span>The conversation of gestures is the beginning of communication.</span></li>
<li><span>The inner conversation is the beginning of self (selfrealization). </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>One inevitably seeks communication with others.</span></li>
<li><span>Communication requires planning.</span></li>
<li><strong><span>Thinking</span></strong><span> becomes preparatory to social action.</span></li>
<li><span>The process of </span><strong><span>thinking is an inner conversation.</span></strong></li>
<li><u><span>Symbols are essential for communication and the development of the self.</span></u><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The </span><strong><span>complete self</span></strong><span> reflects the unity of the social process; and each of the elementary selves reflects the complete social process of self-reflection and interaction with others.</span></li>
<li><span>Stages of the development of the self:</span>
<ol>
<li><u><span>Play stage</span></u><span>: dyatic relationships.</span></li>
<li><u><span>Game stage</span></u><span>: multiple relationships.</span></li>
</ol>
</li>
<li><strong><span>Game playing</span></strong><span> requires a realization of the generalized other: assuming the statuses and roles of all involved. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The self-conscious individual assumes the organized social attitudes of the social group.</span></li>
<li><span>The self is not so much a substance as a process, continually changing and adapting to social processes.</span></li>
<li><span>The </span><strong><span>“me”</span></strong><span> is the accumulated awareness of "</span><em><span>the generalized other.</span></em><span>”</span></li>
<li><span>The </span><strong><span>“I”</span></strong><span> is the more personal. It is the reflector or observer.</span></li>
<li><strong><span>The human mind arises solely through social experience.</span></strong><span> It represents the thinking process of internalized communication. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><hr><h2 id="MIND" data-id="MIND"><a class="anchor hidden-xs" href="#MIND" title="MIND"><span class="octicon octicon-link"></span></a><span>MIND</span></h2><ul>
<li><span>Motivation:</span>
<ul>
<li><span>What is human mind and how does it work? How do we recognize objects and scenes? How do we use words and languages? How do we achieve goals? How do we learn ? How does common sense work?</span></li>
</ul>
</li>
</ul><h3 id="Analogy-An-ants-society" data-id="Analogy-An-ants-society"><a class="anchor hidden-xs" href="#Analogy-An-ants-society" title="Analogy-An-ants-society"><span class="octicon octicon-link"></span></a><span>Analogy: An ants society</span></h3><ul>
<li><span>An individual ant is not very bright, but ants in a colony, operating as a collective, do remarkable things.</span></li>
</ul><blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>A single neuron in the human brain can respond only to what the neurons connected to it are doing, but all of them together can be Albert Einstein. </span><em><span>Deborah M. Gordon (Stanford University)</span></em><span> </span><span class="color" data-color="#37B9BF"></span></p>
</blockquote><ul>
<li><span>Some social systems in Nature can present an </span><em><span>intelligent collective behaviour</span></em><span> although they are composed by simple individuals.</span></li>
<li><span>The intelligent solutions to problems naturally emerge from the self-organization and </span><em><span>communication</span></em><span> of these individuals.</span>
<ul>
<li><span>Carrying large items, forming bridges, finding the shortest routes from the nest to a food source, prioritizing food sources based on their distance and ease of access…</span></li>
</ul>
</li>
<li><span>Individual ants are simple insects with </span><em><strong><span>limited</span></strong></em><span> memory and capable of performing </span><em><strong><span>simple</span></strong></em><span> actions. However, an ant colony expresses a </span><em><strong><span>complex</span></strong></em><span> collective behaviour.</span>
<ul>
<li><span>How do they know which task to perform? How can they manage to find the shortest path (Goal)? How did the Ants communicate with each other? How do they form such huge colonies?</span></li>
</ul>
</li>
<li><span>Ants have dealt with the same kind of questions which we have set out with.</span></li>
</ul><h3 id="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" data-id="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951"><a class="anchor hidden-xs" href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951"><span class="octicon octicon-link"></span></a><span>Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</span></h3><ul>
<li><u><span>Key idea</span></u><span>: producing machines which could learn by providing them with memory neurones connected to synapses; the machine would also have to possess past memory in order to function efficiently when faced with different situations.</span></li>
</ul><h3 id="Marvin-Minsky-The-Society-of-Mind" data-id="Marvin-Minsky-The-Society-of-Mind"><a class="anchor hidden-xs" href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin-Minsky-The-Society-of-Mind"><span class="octicon octicon-link"></span></a><span>Marvin Minsky, The Society of Mind</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>Background</span></u><span>: The functions performed by the brain are the products of the work of thousands of different, specialized sub-systems, the intricate product of hundreds of millions of years of biological evolution. We cannot hope to understand such an organization by emulating the techniques of those particle physicists who search for the simplest possible unifying conceptions. </span><strong><span>Constructing a mind is simply a different kind of problem</span></strong><span>—of how to synthesize organizational systems that can support a large enough diversity of different schemes, yet enable them to work together to exploit one another’s abilities. </span><em><span>[Minsky, M.: Logical vs. Analogical or Symbolic vs. Connectionist or Neat vs. Scruffy.]</span></em></li>
<li><u><span>Aim</span></u><span>: to create a theory of human cognition. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>Approach</span></u><span>: A Cognitive Architecture composed by thousands of individual agents.</span></li>
<li><u><span>Idea</span></u><span>: Human intelligence is built layer by layer from the interactions of simple parts called </span><strong><span>agents</span></strong><span>, which are themselves mindless.</span>
<ul>
<li><span>Theory covers processes </span><strong><span>such as language, memory, learning, consciousness, the sense of self, and free-will.</span></strong></li>
<li><span>Very flexible. Based on integration. Scalable.</span></li>
</ul>
</li>
<li><u><span>Point of view</span></u><span>: constructivist and organicist.</span></li>
<li><u><span>Technical perspective</span></u><span>: Parallelism, different types of Knowledge bases, compatibility between the symbolic and sub-symbolic levels. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>The revolutionary proposal of The Society of Mind:</span></u>
<ul>
<li><span>It takes into account and tries to explain cognitive development.</span></li>
<li><span>It takes into account evolution.</span></li>
<li><span>It takes into account emotions.</span></li>
<li><span>Flexible behaviour depending on the environment.</span></li>
<li><span>Exhibiting some rationality. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</li>
</ul>
</blockquote><hr><h2 id="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" data-id="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for"><a class="anchor hidden-xs" href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for"><span class="octicon octicon-link"></span></a><span>Which Kind of Cognitive Architectures are we Looking for?</span></h2><ul>
<li><span>Capable to operate in rich and complex environments.</span></li>
<li><span>Capable of using symbols and abstractions.</span></li>
<li><span>Use of natural and artificial languages.</span></li>
<li><span>Learn from the environment and the experience.</span></li>
<li><span>Get capabilities during execution time (adaptation).</span></li>
<li><span>Operate in an autonomous way, but being social.</span></li>
<li><span>Be self-conscious.</span></li>
<li><span>Be built from (artificial) neurons.</span></li>
<li><span>Emerge from evolution.</span></li>
</ul><hr><h2 id="Nature-of-the-Brain" data-id="Nature-of-the-Brain"><a class="anchor hidden-xs" href="#Nature-of-the-Brain" title="Nature-of-the-Brain"><span class="octicon octicon-link"></span></a><span>Nature of the Brain</span></h2><ul>
<li><span>Human minds are not perfect decision-makers, but by and large they are very good.</span></li>
<li><span>Brains are not as modular as software.</span></li>
<li><strong><span>Brains may are to </span><em><span>intelligence</span></em><span> as wings to </span><em><span>flying</span></em></strong><span>. Mimesis is not always the best idea.</span></li>
<li><span>Lessons learned: memory and simulation (planning) are good to decision making.</span></li>
</ul><hr><h2 id="Architectures-for-Reactive-Systems" data-id="Architectures-for-Reactive-Systems"><a class="anchor hidden-xs" href="#Architectures-for-Reactive-Systems" title="Architectures-for-Reactive-Systems"><span class="octicon octicon-link"></span></a><span>Architectures for Reactive Systems</span></h2><ul>
<li><span>These systems make decision at run time based on limited information and simple situation action rules.</span></li>
<li><span>These architectures were often called behaviour based, situated or reactive.</span></li>
<li><strong><span>Brooks with Subsumption architecture denied the need for symbolic representation of the world, instead the systems make their decisions based on the inputs.</span></strong></li>
<li><span>The decision of reactive architectures are partly guided by Simon’s hypothesis states that that the </span><em><span>complexity of the behaviour of the system can be a reflection of the complexity of the environment rather than the reflection of the system’s complex internal design.</span></em></li>
</ul><blockquote style="border-left-color: rgb(255, 191, 0);">
<p><strong><em><span>NOTE:</span></em></strong><span>  Cognitive architectures and neural networks are not the same. </span><span class="color" data-color="#FFBF00"></span></p>
</blockquote><hr><h2 id="Cognitive-Architectures-II" data-id="Cognitive-Architectures-II"><a class="anchor hidden-xs" href="#Cognitive-Architectures-II" title="Cognitive-Architectures-II"><span class="octicon octicon-link"></span></a><span>Cognitive Architectures II</span></h2><h3 id="Parameters" data-id="Parameters"><a class="anchor hidden-xs" href="#Parameters" title="Parameters"><span class="octicon octicon-link"></span></a><span>Parameters</span></h3><ul>
<li><span>Generality</span></li>
<li><span>Versatility</span></li>
<li><span>Rationality</span></li>
<li><span>Learning</span></li>
<li><span>Psychological Validation</span></li>
<li><span>Applicability</span></li>
<li><span>Scalability</span></li>
<li><span>Reactivity</span></li>
<li><span>Efficiency</span></li>
</ul><h3 id="Open-issues" data-id="Open-issues"><a class="anchor hidden-xs" href="#Open-issues" title="Open-issues"><span class="octicon octicon-link"></span></a><span>Open issues</span></h3><ul>
<li><span>Which is the best of all Architectures?</span></li>
<li><span>Will we ever get complete architectures?</span></li>
<li><span>Which kind of intelligence will we get?</span></li>
<li><span>How can agents solve problems?</span></li>
</ul><h3 id="Functional-aspects" data-id="Functional-aspects"><a class="anchor hidden-xs" href="#Functional-aspects" title="Functional-aspects"><span class="octicon octicon-link"></span></a><span>Functional aspects</span></h3><ul>
<li><span>Engineering methodology (how to develop them).</span></li>
<li><span>Capability to tackle a wide range of complex tasks.</span></li>
<li><span>Efficiency when acting on the environment.</span></li>
<li><span>Autonomy.</span></li>
</ul><hr><h2 id="Rational-Decisions" data-id="Rational-Decisions"><a class="anchor hidden-xs" href="#Rational-Decisions" title="Rational-Decisions"><span class="octicon octicon-link"></span></a><span>Rational Decisions</span></h2><ul>
<li><strong><span>Rational</span></strong><span>: maximally achieving pre-defined goals.</span></li>
<li><span>Rationality only concerns what decisions are made.</span></li>
<li><strong><span>Goals</span></strong><span> are expressed in terms of utility (of outcomes).</span></li>
</ul><figure>
<img src="https://i.imgur.com/9ErCMOo.png">
<figcaption><b>What kind of AI?</b></figcaption>
</figure><blockquote>
<p><em><span>I think the big problem is that we’re not smart enough to understand which of the problems we’re facing are good enough. Therefore, we have to build super intelligent machines like HAL.</span></em><span> -Marvin Minsky</span></p>
</blockquote></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
<li class=""><a href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction to Distributed Intelligent Agent Systems">Introduction to Distributed Intelligent Agent Systems</a><ul class="nav">
<li><a href="#Artificial-Intelligence" title="Artificial Intelligence">Artificial Intelligence</a></li>
<li><a href="#Cognitive-Architectures-I" title="Cognitive Architectures I">Cognitive Architectures I</a></li>
<li><a href="#Intelligent-Agent" title="Intelligent Agent">Intelligent Agent</a></li>
<li><a href="#Cognitive-AI-Paradigms" title="Cognitive AI Paradigms">Cognitive AI Paradigms</a></li>
<li><a href="#Cognitive-AI-Fundations" title="Cognitive AI Fundations">Cognitive AI Fundations</a><ul class="nav">
<li><a href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George Herbert Mead (1863-1931) Mind, Self, and Society">George Herbert Mead (1863-1931) Mind, Self, and Society</a></li>
</ul>
</li>
<li><a href="#MIND" title="MIND">MIND</a><ul class="nav">
<li><a href="#Analogy-An-ants-society" title="Analogy: An ants society">Analogy: An ants society</a></li>
<li><a href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)">Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</a></li>
<li><a href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin Minsky, The Society of Mind">Marvin Minsky, The Society of Mind</a></li>
</ul>
</li>
<li class=""><a href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which Kind of Cognitive Architectures are we Looking for?">Which Kind of Cognitive Architectures are we Looking for?</a></li>
<li><a href="#Nature-of-the-Brain" title="Nature of the Brain">Nature of the Brain</a></li>
<li><a href="#Architectures-for-Reactive-Systems" title="Architectures for Reactive Systems">Architectures for Reactive Systems</a></li>
<li><a href="#Cognitive-Architectures-II" title="Cognitive Architectures II">Cognitive Architectures II</a><ul class="nav">
<li><a href="#Parameters" title="Parameters">Parameters</a></li>
<li><a href="#Open-issues" title="Open issues">Open issues</a></li>
<li><a href="#Functional-aspects" title="Functional aspects">Functional aspects</a></li>
</ul>
</li>
<li><a href="#Rational-Decisions" title="Rational Decisions">Rational Decisions</a></li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
            </ul>
        </div>
    </div>
    <div id="ui-toc-affix" class="ui-affix-toc ui-toc-dropdown unselectable hidden-print" data-spy="affix" style="top:17px;display:none;" null null>
        <div class="toc"><ul class="nav">
<li class=""><a href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction to Distributed Intelligent Agent Systems">Introduction to Distributed Intelligent Agent Systems</a><ul class="nav">
<li><a href="#Artificial-Intelligence" title="Artificial Intelligence">Artificial Intelligence</a></li>
<li><a href="#Cognitive-Architectures-I" title="Cognitive Architectures I">Cognitive Architectures I</a></li>
<li><a href="#Intelligent-Agent" title="Intelligent Agent">Intelligent Agent</a></li>
<li><a href="#Cognitive-AI-Paradigms" title="Cognitive AI Paradigms">Cognitive AI Paradigms</a></li>
<li><a href="#Cognitive-AI-Fundations" title="Cognitive AI Fundations">Cognitive AI Fundations</a><ul class="nav">
<li><a href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George Herbert Mead (1863-1931) Mind, Self, and Society">George Herbert Mead (1863-1931) Mind, Self, and Society</a></li>
</ul>
</li>
<li><a href="#MIND" title="MIND">MIND</a><ul class="nav">
<li><a href="#Analogy-An-ants-society" title="Analogy: An ants society">Analogy: An ants society</a></li>
<li><a href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)">Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</a></li>
<li><a href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin Minsky, The Society of Mind">Marvin Minsky, The Society of Mind</a></li>
</ul>
</li>
<li class=""><a href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which Kind of Cognitive Architectures are we Looking for?">Which Kind of Cognitive Architectures are we Looking for?</a></li>
<li><a href="#Nature-of-the-Brain" title="Nature of the Brain">Nature of the Brain</a></li>
<li><a href="#Architectures-for-Reactive-Systems" title="Architectures for Reactive Systems">Architectures for Reactive Systems</a></li>
<li><a href="#Cognitive-Architectures-II" title="Cognitive Architectures II">Cognitive Architectures II</a><ul class="nav">
<li><a href="#Parameters" title="Parameters">Parameters</a></li>
<li><a href="#Open-issues" title="Open issues">Open issues</a></li>
<li><a href="#Functional-aspects" title="Functional aspects">Functional aspects</a></li>
</ul>
</li>
<li><a href="#Rational-Decisions" title="Rational Decisions">Rational Decisions</a></li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js" integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8=" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha256-U5ZEeKfGNOja007MMD3YBI0A3OSZOQbeG6z2f2Y0hu8=" crossorigin="anonymous" defer></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gist-embed/2.6.0/gist-embed.min.js" integrity="sha256-KyF2D6xPIJUW5sUDSs93vWyZm+1RzIpKCexxElmxl8g=" crossorigin="anonymous" defer></script>
    <script>
        var markdown = $(".markdown-body");
        //smooth all hash trigger scrolling
        function smoothHashScroll() {
            var hashElements = $("a[href^='#']").toArray();
            for (var i = 0; i < hashElements.length; i++) {
                var element = hashElements[i];
                var $element = $(element);
                var hash = element.hash;
                if (hash) {
                    $element.on('click', function (e) {
                        // store hash
                        var hash = this.hash;
                        if ($(hash).length <= 0) return;
                        // prevent default anchor click behavior
                        e.preventDefault();
                        // animate
                        $('body, html').stop(true, true).animate({
                            scrollTop: $(hash).offset().top
                        }, 100, "linear", function () {
                            // when done, add hash to url
                            // (default click behaviour)
                            window.location.hash = hash;
                        });
                    });
                }
            }
        }

        smoothHashScroll();
        var toc = $('.ui-toc');
        var tocAffix = $('.ui-affix-toc');
        var tocDropdown = $('.ui-toc-dropdown');
        //toc
        tocDropdown.click(function (e) {
            e.stopPropagation();
        });

        var enoughForAffixToc = true;

        function generateScrollspy() {
            $(document.body).scrollspy({
                target: ''
            });
            $(document.body).scrollspy('refresh');
            if (enoughForAffixToc) {
                toc.hide();
                tocAffix.show();
            } else {
                tocAffix.hide();
                toc.show();
            }
            $(document.body).scroll();
        }

        function windowResize() {
            //toc right
            var paddingRight = parseFloat(markdown.css('padding-right'));
            var right = ($(window).width() - (markdown.offset().left + markdown.outerWidth() - paddingRight));
            toc.css('right', right + 'px');
            //affix toc left
            var newbool;
            var rightMargin = (markdown.parent().outerWidth() - markdown.outerWidth()) / 2;
            //for ipad or wider device
            if (rightMargin >= 133) {
                newbool = true;
                var affixLeftMargin = (tocAffix.outerWidth() - tocAffix.width()) / 2;
                var left = markdown.offset().left + markdown.outerWidth() - affixLeftMargin;
                tocAffix.css('left', left + 'px');
            } else {
                newbool = false;
            }
            if (newbool != enoughForAffixToc) {
                enoughForAffixToc = newbool;
                generateScrollspy();
            }
        }
        $(window).resize(function () {
            windowResize();
        });
        $(document).ready(function () {
            windowResize();
            generateScrollspy();
        });

        //remove hash
        function removeHash() {
            window.location.hash = '';
        }

        var backtotop = $('.back-to-top');
        var gotobottom = $('.go-to-bottom');

        backtotop.click(function (e) {
            e.preventDefault();
            e.stopPropagation();
            if (scrollToTop)
                scrollToTop();
            removeHash();
        });
        gotobottom.click(function (e) {
            e.preventDefault();
            e.stopPropagation();
            if (scrollToBottom)
                scrollToBottom();
            removeHash();
        });

        var toggle = $('.expand-toggle');
        var tocExpand = false;

        checkExpandToggle();
        toggle.click(function (e) {
            e.preventDefault();
            e.stopPropagation();
            tocExpand = !tocExpand;
            checkExpandToggle();
        })

        function checkExpandToggle () {
            var toc = $('.ui-toc-dropdown .toc');
            var toggle = $('.expand-toggle');
            if (!tocExpand) {
                toc.removeClass('expand');
                toggle.text('Expand all');
            } else {
                toc.addClass('expand');
                toggle.text('Collapse all');
            }
        }

        function scrollToTop() {
            $('body, html').stop(true, true).animate({
                scrollTop: 0
            }, 100, "linear");
        }

        function scrollToBottom() {
            $('body, html').stop(true, true).animate({
                scrollTop: $(document.body)[0].scrollHeight
            }, 100, "linear");
        }
    </script>
</body>

</html>
