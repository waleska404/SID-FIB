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
        Introducción a JADE - HackMD
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
    <div id="doc" class="markdown-body container-fluid comment-inner comment-enabled" data-hard-breaks="true"><h1 id="Introducción-a-JADE" data-id="Introducción-a-JADE"><a class="anchor hidden-xs" href="#Introducción-a-JADE" title="Introducción-a-JADE"><span class="octicon octicon-link"></span></a><span>Introducción a JADE</span></h1><h6 id="tags-SID-lab" data-id="tags-SID-lab"><a class="anchor hidden-xs" href="#tags-SID-lab" title="tags-SID-lab"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-lab</code></h6><p><span class="toc"><ul>
<li><a href="#Introducción-a-JADE" title="Introducción a JADE">Introducción a JADE</a><ul>
<li><a href="#Setup-del-entorno" title="Setup del entorno">Setup del entorno</a></li>
<li><a href="#Agentes" title="Agentes">Agentes</a><ul>
<li><a href="#Nombres-locales-GUID-y-direcciones" title="Nombres locales, GUID y direcciones">Nombres locales, GUID y direcciones</a></li>
<li><a href="#Paso-de-parámetros" title="Paso de parámetros">Paso de parámetros</a></li>
<li><a href="#Expiración-del-agente" title="Expiración del agente">Expiración del agente</a></li>
<li><a href="#Construyendo-un-agente" title="Construyendo un agente">Construyendo un agente</a></li>
<li><a href="#Ciclo-de-vida-del-agente" title="Ciclo de vida del agente">Ciclo de vida del agente</a></li>
<li><a href="#Estados-del-agente" title="Estados del agente">Estados del agente</a></li>
</ul>
</li>
<li><a href="#Comportamientos-Behaviours" title="Comportamientos (Behaviours)">Comportamientos (Behaviours)</a><ul>
<li><a href="#Planificación-y-ejecución-de-Behaviours" title="Planificación y ejecución de Behaviours">Planificación y ejecución de Behaviours</a></li>
<li><a href="#Tipos-de-Behaviours" title="Tipos de Behaviours">Tipos de Behaviours</a></li>
<li><a href="#Empezar-y-acabar-los-Behaviours" title="Empezar y acabar los Behaviours">Empezar y acabar los Behaviours</a></li>
</ul>
</li>
<li><a href="#Directory-Facilitator-DF" title="Directory Facilitator (DF)">Directory Facilitator (DF)</a><ul>
<li><a href="#Registro" title="Registro">Registro</a></li>
<li><a href="#Búsqueda" title="Búsqueda">Búsqueda</a></li>
</ul>
</li>
<li><a href="#Modelo-de-comunicación" title="Modelo de comunicación">Modelo de comunicación</a><ul>
<li><a href="#La-clase-ACLMessage" title="La clase ACLMessage">La clase ACLMessage</a></li>
<li><a href="#Envío-y-recepción-de-mensajes" title="Envío y recepción de mensajes">Envío y recepción de mensajes</a></li>
<li><a href="#Message-templates" title="Message templates">Message templates</a></li>
<li><a href="#Paso-de-mensajes" title="Paso de mensajes">Paso de mensajes</a></li>
<li><a href="#Protocolos-de-interacción" title="Protocolos de interacción">Protocolos de interacción</a></li>
<li><a href="#Soporte-a-los-protocolos-de-interacción" title="Soporte a los protocolos de interacción">Soporte a los protocolos de interacción</a></li>
<li><a href="#AchieveREInitiatorResponder" title="AchieveREInitiator/Responder">AchieveREInitiator/Responder</a></li>
<li><a href="#FIPA-Contract-Net-protocol" title="FIPA Contract-Net protocol">FIPA Contract-Net protocol</a></li>
</ul>
</li>
<li><a href="#Gestión-de-contenido" title="Gestión de contenido">Gestión de contenido</a><ul>
<li><a href="#ACL-Message" title="ACL Message">ACL Message</a></li>
<li><a href="#Content-Manager" title="Content Manager">Content Manager</a></li>
<li><a href="#Ontología-para-JADE" title="Ontología para JADE">Ontología para JADE</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</span></p><hr><ul>
<li><strong><span>Referencias</span></strong><span>:</span>
<ul>
<li><a href="http://jade.tilab.com/documentation/tutorials-guides/" target="_blank" rel="noopener"><span>http://jade.tilab.com/documentation/tutorials-guides/</span></a>
<ul>
<li><span>JADE Administrador’s Guide</span></li>
<li><span>JADE Programming for Beginners</span></li>
</ul>
</li>
<li><a href="http://jade.tilab.com/documentation/examples/" target="_blank" rel="noopener"><span>http://jade.tilab.com/documentation/examples/</span></a></li>
</ul>
</li>
</ul><hr><h2 id="Setup-del-entorno" data-id="Setup-del-entorno"><a class="anchor hidden-xs" href="#Setup-del-entorno" title="Setup-del-entorno"><span class="octicon octicon-link"></span></a><span>Setup del entorno</span></h2><ul>
<li><span>Descargas:</span>
<ul>
<li><span>jade.jar: </span><a href="https://jade.tilab.com/dl.php?file=JADE-all-4.5.0.zip" target="_blank" rel="noopener"><span>https://jade.tilab.com/dl.php?file=JADE-all-4.5.0.zip</span></a></li>
<li><span>commons-codec-1.3.jar: </span><a href="https://repo1.maven.org/maven2/commons-codec/commons-codec/1.3/commons-codec-1.3.jar" target="_blank" rel="noopener"><span>https://repo1.maven.org/maven2/commons-codec/commons-codec/1.3/commons-codec-1.3.jar</span></a></li>
<li><span>ejemplos: </span><a href="https://gitlab.fib.upc.edu/sergio.alvarez-napagao/material-sid" target="_blank" rel="noopener"><span>https://gitlab.fib.upc.edu/sergio.alvarez-napagao/material-sid</span></a></li>
</ul>
</li>
<li><span>Configuración del CLASSPATH:</span>
<ul>
<li><code>JADE-all-4.5.0/JADE-bin-4.5.0/jade/lib/jade.jar</code></li>
<li><span>commons-codec-1.3.jar</span></li>
<li><span>Directorio que guarda los .class (e.g. </span><code>output/ o classes/</code><span>)</span></li>
<li><code>export CLASSPATH="$CLASSPATH:&lt;JARS_AND_FOLDERS&gt;"</code></li>
</ul>
</li>
<li><span>Arrancamos la GUI:</span>
<ul>
<li><code>java jade.Boot –gui</code></li>
<li><span>Si no tenemos el CLASSPATH siempre podemos usar </span><code>–cp u java –cp lib/jade.jar jade.Boot –gui</code></li>
</ul>
</li>
</ul><hr><h2 id="Agentes" data-id="Agentes"><a class="anchor hidden-xs" href="#Agentes" title="Agentes"><span class="octicon octicon-link"></span></a><span>Agentes</span></h2><ul>
<li><span>Una clase de agente se crea:</span>
<ul>
<li><span>Extendiendo la clase </span><code>jade.core.Agent</code></li>
<li><span>Y redefiniendo el método </span><code>setup()</code></li>
</ul>
</li>
<li><span>Cada instancia se identifica con un AID (</span><code>jade.core.AID</code><span>)</span>
<ul>
<li><span>AID: se compone de un nombre único más la dirección de la plataforma</span></li>
<li><span>Podemos recuperar el AID de un agente mediante el método </span><code>getAID()</code><span> de la clase </span><code>Agent</code></li>
</ul>
</li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token keyword">import</span> <span class="token namespace">jade<span class="token punctuation">.</span>core<span class="token punctuation">.</span></span><span class="token class-name">Agent</span><span class="token punctuation">;</span>

<span class="token keyword">public</span> <span class="token keyword">class</span> <span class="token class-name">HelloWorldAgent</span> <span class="token keyword">extends</span> <span class="token class-name">Agent</span> <span class="token punctuation">{</span>
    
    <span class="token keyword">protected</span> <span class="token keyword">void</span> <span class="token function">setup</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span>println<span class="token punctuation">.</span><span class="token punctuation">(</span><span class="token string">"Hello World! my name is "</span> <span class="token operator">+</span> <span class="token function">getAID</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">getName</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Nombres-locales-GUID-y-direcciones" data-id="Nombres-locales-GUID-y-direcciones"><a class="anchor hidden-xs" href="#Nombres-locales-GUID-y-direcciones" title="Nombres-locales-GUID-y-direcciones"><span class="octicon octicon-link"></span></a><span>Nombres locales, GUID y direcciones</span></h3><ul>
<li><span>Nombre agente: </span><code>&lt;nombre-local&gt;@&lt;nombre-plataforma&gt;</code>
<ul>
<li><span>Nombre-local es único (localmente).</span></li>
<li><span>El nombre completo ha de ser único globalmente.</span></li>
</ul>
</li>
<li><span>Para especificar el nombre de la plataforma al arrancarla: opción </span><code>–name</code></li>
<li><span>Dentro de la plataforma nos referimos al agente usando únicamente su nombre-local</span></li>
</ul><pre style="position: relative;"><code class="java hljs"><span class="token class-name">AID</span> localId <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token function">AID</span><span class="token punctuation">(</span>localname<span class="token punctuation">,</span> AID<span class="token punctuation">.</span>ISLOCALNAME<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token class-name">AID</span> globalId <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token function">AID</span><span class="token punctuation">(</span>name<span class="token punctuation">,</span> AID<span class="token punctuation">.</span>ISGUID<span class="token punctuation">)</span><span class="token punctuation">;</span>
</code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Paso-de-parámetros" data-id="Paso-de-parámetros"><a class="anchor hidden-xs" href="#Paso-de-parámetros" title="Paso-de-parámetros"><span class="octicon octicon-link"></span></a><span>Paso de parámetros</span></h3><ul>
<li><span>Pasar parámetros a un agente: </span><code>java jade.Boot .. ´A:myPackage.MyAgent(arg1 arg2)´</code></li>
<li><span>Recuperar los argumentos con el método </span><code>getArguments()</code><span> de la clase </span><code>Agent</code></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token keyword">protected</span> <span class="token keyword">void</span> <span class="token function">setup</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">Object</span><span class="token punctuation">[</span><span class="token punctuation">]</span> args <span class="token operator">=</span> <span class="token function">getArguments</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token keyword">if</span> <span class="token punctuation">(</span>args <span class="token operator">!=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"Hello, my arguments are:"</span><span class="token punctuation">)</span>
        <span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">int</span> i <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span> i <span class="token operator">&lt;</span> args<span class="token punctuation">.</span>length<span class="token punctuation">;</span> <span class="token operator">++</span>i<span class="token punctuation">)</span> <span class="token punctuation">{</span>
            <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"- "</span> <span class="token operator">+</span> args<span class="token punctuation">[</span>i<span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token punctuation">}</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Expiración-del-agente" data-id="Expiración-del-agente"><a class="anchor hidden-xs" href="#Expiración-del-agente" title="Expiración-del-agente"><span class="octicon octicon-link"></span></a><span>Expiración del agente</span></h3><ul>
<li><span>El agente termina su ejecución cuando se llama a su método </span><code>doDelete()</code></li>
<li><span>Durante su terminación se invoca el método </span><code>takeDown()</code><span> (e.g., para realizar operaciones de limpieza)</span></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token keyword">protected</span> <span class="token keyword">void</span> <span class="token function">setup</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span>println<span class="token punctuation">.</span><span class="token punctuation">(</span><span class="token string">"Hello World! my name is "</span> <span class="token operator">+</span> <span class="token function">getAID</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">getName</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token class-name">Object</span><span class="token punctuation">[</span><span class="token punctuation">]</span> args <span class="token operator">=</span> <span class="token function">getArguments</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token keyword">if</span> <span class="token punctuation">(</span>args <span class="token operator">!=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"Hello, my arguments are:"</span><span class="token punctuation">)</span>
        <span class="token keyword">for</span> <span class="token punctuation">(</span><span class="token keyword">int</span> i <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">;</span> i <span class="token operator">&lt;</span> args<span class="token punctuation">.</span>length<span class="token punctuation">;</span> <span class="token operator">++</span>i<span class="token punctuation">)</span> <span class="token punctuation">{</span>
            <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"- "</span> <span class="token operator">+</span> args<span class="token punctuation">[</span>i<span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
        <span class="token punctuation">}</span>
    <span class="token punctuation">}</span>
    <span class="token function">doDelete</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>

<span class="token keyword">protected</span> <span class="token keyword">void</span> <span class="token function">takeDown</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">System</span><span class="token punctuation">.</span>out<span class="token punctuation">.</span><span class="token function">println</span><span class="token punctuation">(</span><span class="token string">"Bye..."</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>

</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Construyendo-un-agente" data-id="Construyendo-un-agente"><a class="anchor hidden-xs" href="#Construyendo-un-agente" title="Construyendo-un-agente"><span class="octicon octicon-link"></span></a><span>Construyendo un agente</span></h3><ul>
<li><code>setup()</code><span>: método para preparar el agente; se ejecuta una vez.</span>
<ul>
<li><span>Registro en el DF.</span></li>
<li><span>Iniciar todos los behaviours requeridos.</span></li>
<li><span>Es obligatorio que haya al menos un behaviour en el setup.</span></li>
</ul>
</li>
<li><code>takeDown()</code><span>: al finalizar el agente</span>
<ul>
<li><span>Eliminar del registro del DF.</span></li>
<li><span>Cerrar todos los recursos abiertos/requeridos…</span></li>
</ul>
</li>
</ul><h3 id="Ciclo-de-vida-del-agente" data-id="Ciclo-de-vida-del-agente"><a class="anchor hidden-xs" href="#Ciclo-de-vida-del-agente" title="Ciclo-de-vida-del-agente"><span class="octicon octicon-link"></span></a><span>Ciclo de vida del agente</span></h3><center><img src="https://i.imgur.com/t3w0h4y.png"></center><h3 id="Estados-del-agente" data-id="Estados-del-agente"><a class="anchor hidden-xs" href="#Estados-del-agente" title="Estados-del-agente"><span class="octicon octicon-link"></span></a><span>Estados del agente</span></h3><table>
<thead>
<tr>
<th><span>State</span></th>
<th><span>Description</span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span>Initiated</span></td>
<td><span>The agent object is built, but hasn’t registered itself with AMS, has neither name nor an addressand can’t communicate with other agents.</span></td>
</tr>
<tr>
<td><span>Active</span></td>
<td><span>The agent object is registered with AMS, has regular name and address, can access all the various JADE features.</span></td>
</tr>
<tr>
<td><span>Suspended</span></td>
<td><span>The agent object is currently stopped. Its internal thread is suspended and no agent behaviour is being executed.</span></td>
</tr>
<tr>
<td><span>Waiting</span></td>
<td><span>The agent is blocked, waiting for something. Its internal thread is sleeping on a JAVA monitor and will wake up when some conditions are met (for example when message arrives).</span></td>
</tr>
<tr>
<td><span>Deleted</span></td>
<td><span>The agent is definitely dead. The internal thread has terminated its execution and the agent is no more registered with AMS.</span></td>
</tr>
<tr>
<td><span>Transit</span></td>
<td><span>The mobile agent enters this state while it is migrating to the new location. The system continues to buffer messages that will then be sent to its new location.</span></td>
</tr>
</tbody>
</table><center><img src="https://i.imgur.com/LeeXD7Y.png"></center><hr><h2 id="Comportamientos-Behaviours" data-id="Comportamientos-Behaviours"><a class="anchor hidden-xs" href="#Comportamientos-Behaviours" title="Comportamientos-Behaviours"><span class="octicon octicon-link"></span></a><span>Comportamientos (</span><em><span>Behaviours</span></em><span>)</span></h2><ul>
<li><span>Los agentes realizan sus tareas mediante </span><em><span>behaviours</span></em><span>.</span></li>
<li><span>Los </span><em><span>behaviours</span></em><span> se crean extendiendo la clase</span><code>jade.core.behaviours.Behaviour</code></li>
<li><span>Para que un agente ejecute una tarea basta con:</span>
<ul>
<li><span>Crear una instancia de la subclase </span><code>Behaviour</code><span> correspondiente.</span></li>
<li><span>Llamar al método </span><code>addBehaviour()</code><span> de la clase </span><code>Agent</code></li>
</ul>
</li>
<li><span>Cada </span><em><span>behaviour</span></em><span> debe implementar:</span>
<ul>
<li><code>public void action()</code><span>: Qué hace el </span><em><span>behaviour</span></em><span>.</span></li>
<li><code>public boolean done()</code><span>: Cierto si ya ha finalizado.</span></li>
</ul>
</li>
</ul><h3 id="Planificación-y-ejecución-de-Behaviours" data-id="Planificación-y-ejecución-de-Behaviours"><a class="anchor hidden-xs" href="#Planificación-y-ejecución-de-Behaviours" title="Planificación-y-ejecución-de-Behaviours"><span class="octicon octicon-link"></span></a><span>Planificación y ejecución de Behaviours</span></h3><ul>
<li><span>Un agente puede ejecutar varios comportamientos en paralelo.</span></li>
<li><span>La planificación de estas ejecuciones no es </span><strong><span>preferente</span></strong><span>.</span>
<ul>
<li><span>No es determinista a la hora de seleccionar un behaviour si hay varios disponibles.</span>
<ul>
<li><span>Cola con round-robin con planificación colaborativa.</span></li>
</ul>
</li>
</ul>
</li>
<li><span>Todo ocurre en el mismo thread de Java.</span></li>
<li><span>Los cambios de behaviour a ejecutar ocurren cuando el método </span><code>action</code><span> del behaviour que se está ejecutando finaliza.</span></li>
</ul><h3 id="Tipos-de-Behaviours" data-id="Tipos-de-Behaviours"><a class="anchor hidden-xs" href="#Tipos-de-Behaviours" title="Tipos-de-Behaviours"><span class="octicon octicon-link"></span></a><span>Tipos de Behaviours</span></h3><ul>
<li>
<h4 id="Heredan-de-la-clase-SimpleBehaviour" data-id="Heredan-de-la-clase-SimpleBehaviour"><a class="anchor hidden-xs" href="#Heredan-de-la-clase-SimpleBehaviour" title="Heredan-de-la-clase-SimpleBehaviour"><span class="octicon octicon-link"></span></a><u><span>Heredan de la clase </span><code>SimpleBehaviour</code><span>:</span></u></h4>
<ul>
<li><strong><span>One shot</span></strong><span> (</span><code>jade.core.behaviours.OneShotBehaviour</code><span>)</span>
<ul>
<li><code>action()</code><span>: se ejecuta una vez (se completa inmediatamente).</span></li>
<li><code>done()</code><span>: simplemente devuelve </span><code>true</code><span>.</span></li>
</ul>
</li>
<li><strong><span>Cyclic</span></strong><span> (</span><code>jade.core.behaviours.CyclicBehaviour</code><span>)</span>
<ul>
<li><code>action()</code><span>: ejecuta la misma operación cada vez que se invoca (nunca se completa).</span></li>
<li><code>done()</code><span>: simplemente devuelve </span><code>false</code><span>.</span></li>
</ul>
</li>
<li><strong><span>Waker</span></strong><span> (</span><code>jade.core.behaviours.WakerBehaviour</code><span>)</span>
<ul>
<li><code>onWake()</code><span>: a implementar en las subclases, se ejecuta tras un tiempo dado (timeout).</span></li>
<li><code>action()</code><span> y </span><code>done()</code><span>: ya están implementados para que el método </span><code>onWake()</code><span> se ejecute tras el timeout.</span></li>
<li><span>Tras su ejecución, el </span><em><span>behaviour</span></em><span> queda completado.</span></li>
</ul>
</li>
<li><strong><span>Ticker</span></strong><span> (</span><code>jade.core.behaviours.TickerBehaviour</code><span>)</span>
<ul>
<li><code>onTick()</code><span>: a implementar en las subclases, se ejecuta periódicamente según un periodo dado.</span></li>
<li><code>action()</code><span> y </span><code>done()</code><span>: ya están implementados para que el método </span><code>onTick()</code><span> se ejecute a cada periodo.</span></li>
<li><span>El </span><em><span>behaviour</span></em><span> se ejecuta para siempre a menos que se ejecute su método </span><code>stop()</code></li>
</ul>
</li>
</ul>
</li>
<li>
<h4 id="Heredan-de-la-clase-CompositeBehaviour" data-id="Heredan-de-la-clase-CompositeBehaviour"><a class="anchor hidden-xs" href="#Heredan-de-la-clase-CompositeBehaviour" title="Heredan-de-la-clase-CompositeBehaviour"><span class="octicon octicon-link"></span></a><u><span>Heredan de la clase </span><code>CompositeBehaviour</code><span>:</span></u></h4>
<ul>
<li><code>SequentialBehaviour</code><span>: Ejecuta todos los </span><em><span>sub-behaviours</span></em><span> secuencialmente.</span></li>
<li><code>ParallelBehaviour</code><span>: Ejecuta todos los </span><em><span>sub-behaviours</span></em><span> asíncronamente.</span></li>
<li><code>FSMBehaviour</code><span>: Ejecuta todos los </span><em><span>sub-behaviours</span></em><span> definiendo una máquina de estados.</span></li>
<li><span>Utilizaremos el método</span><code> addSubBehaviour(Behaviour b)</code></li>
</ul>
</li>
</ul><h3 id="Empezar-y-acabar-los-Behaviours" data-id="Empezar-y-acabar-los-Behaviours"><a class="anchor hidden-xs" href="#Empezar-y-acabar-los-Behaviours" title="Empezar-y-acabar-los-Behaviours"><span class="octicon octicon-link"></span></a><span>Empezar y acabar los Behaviours</span></h3><ul>
<li><code>onStart()</code>
<ul>
<li><span>Se ejecuta una vez antes de ejecutar el método </span><code>action()</code></li>
<li><span>Indicado para operaciones que tengan que ocurrir al inicio del </span><em><span>behaviour</span></em><span>.</span></li>
</ul>
</li>
<li><code>onEnd()</code>
<ul>
<li><span>Se ejecuta una vez después de que el método </span><code>done()</code><span> devuelva </span><code>true</code></li>
<li><span>Indicado para operaciones que tengan que ocurrir al final del behaviour.</span></li>
</ul>
</li>
<li><span>Cada behaviour tiene un apuntador al agente que lo ejecuta: el atributo protegido </span><code>myAgent</code></li>
<li><code>removeBehaviour()</code>
<ul>
<li><span>Elimina un </span><em><span>behaviour</span></em><span> del pool de </span><em><span>behaviours</span></em><span> de un agente.</span></li>
<li><span>No se llama al método </span><code>onEnd()</code></li>
</ul>
</li>
<li><span>Cuando el </span><em><span>pool</span></em><span> de </span><em><span>behaviours</span></em><span> de un agente está vacío, el agente pasa a un estado inactivo (IDLE state) y su thread entra en modo </span><em><span>sleep</span></em><span>.</span></li>
</ul><hr><h2 id="Directory-Facilitator-DF" data-id="Directory-Facilitator-DF"><a class="anchor hidden-xs" href="#Directory-Facilitator-DF" title="Directory-Facilitator-DF"><span class="octicon octicon-link"></span></a><span>Directory Facilitator (DF)</span></h2><ul>
<li><span>Recordad que el DF es un agente también.</span></li>
<li><span>Clase </span><code>jade.domain.DFService</code>
<ul>
<li><code>register()</code></li>
<li><code>modify()</code></li>
<li><code>deregister()</code></li>
<li><code>search()</code></li>
</ul>
</li>
</ul><center><img src="https://i.imgur.com/C2ir6Oo.png"></center><h3 id="Registro" data-id="Registro"><a class="anchor hidden-xs" href="#Registro" title="Registro"><span class="octicon octicon-link"></span></a><span>Registro</span></h3><ul>
<li><span>Normalmente en el setup nos registraremos en el DF.</span>
<ul>
<li><span>Usaremos un </span><code>DFAgentDescription</code><span> para indicar:</span>
<ul>
<li><span>el ID del agente (</span><code>getAID()</code><span>).</span></li>
<li><span>los servicios que ofrece.</span></li>
</ul>
</li>
<li><span>Usaremos un </span><code>ServiceDescription</code><span> para cada servicio, indicando:</span>
<ul>
<li><span>el nombre del servicio (</span><code>string</code><span>).</span></li>
<li><span>el tipo de servicio (</span><code>string</code><span>).</span></li>
<li><span>una ontología (opcional).</span></li>
<li><span>un lenguaje del contenido (e.g., FIPA_SL, también opcional).</span></li>
</ul>
</li>
</ul>
</li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token class-name">DFAgentDescription</span> dfd <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">DFAgentDescription</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
dfd<span class="token punctuation">.</span><span class="token function">setName</span><span class="token punctuation">(</span><span class="token function">getAID</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token class-name">ServiceDescription</span> sd <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">ServiceDescription</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
sd<span class="token punctuation">.</span><span class="token function">setName</span><span class="token punctuation">(</span>serviceName<span class="token punctuation">)</span><span class="token punctuation">;</span>
sd<span class="token punctuation">.</span><span class="token function">setType</span><span class="token punctuation">(</span><span class="token string">"weather-forecast"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token comment">// Agents that want to use this service need to</span>
<span class="token comment">// "know" the weather-forecast-ontology</span>
sd<span class="token punctuation">.</span><span class="token function">addOntologies</span><span class="token punctuation">(</span><span class="token string">"weather-forecast-ontology"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token comment">// Agents that want to use this service need to</span>
<span class="token comment">// "speak" the FIPA-SL language</span>
sd<span class="token punctuation">.</span><span class="token function">addLanguages</span><span class="token punctuation">(</span><span class="token class-name">FIPANames<span class="token punctuation">.</span>ContentLanguage</span><span class="token punctuation">.</span>FIPA_SL<span class="token punctuation">)</span><span class="token punctuation">;</span>
sd<span class="token punctuation">.</span><span class="token function">addProperties</span><span class="token punctuation">(</span><span class="token keyword">new</span> <span class="token class-name">Property</span><span class="token punctuation">(</span><span class="token string">"country"</span><span class="token punctuation">,</span> <span class="token string">"Italy"</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
dfd<span class="token punctuation">.</span><span class="token function">addServices</span><span class="token punctuation">(</span>sd<span class="token punctuation">)</span><span class="token punctuation">;</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Búsqueda" data-id="Búsqueda"><a class="anchor hidden-xs" href="#Búsqueda" title="Búsqueda"><span class="octicon octicon-link"></span></a><span>Búsqueda</span></h3><ul>
<li><span>Usaremos un </span><code>DFAgentDescription</code><span> y un </span><code>ServiceDescription</code><span> como template del agente/servicio que buscamos.</span></li>
<li><span>Usaremos un </span><code>SearchConstraints</code><span> para añadir restricciones a la búsqueda (como la cantidad de resultados).</span></li>
<li><span>Enviaremos una petición de búsqueda al </span><code>DFService</code></li>
<li><span>De los resultados obtendremos el AID del proveedor.</span></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token comment">// Build the description used as template for the search</span>
<span class="token class-name">DFAgentDescription</span> template <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">DFAgentDescription</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token class-name">ServiceDescription</span> templateSd <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">ServiceDescription</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
templateSd<span class="token punctuation">.</span><span class="token function">setType</span><span class="token punctuation">(</span><span class="token string">"weather-forecast"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
template<span class="token punctuation">.</span><span class="token function">addServices</span><span class="token punctuation">(</span>templateSd<span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token class-name">SearchConstraints</span> sc <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">SearchConstraints</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token comment">// We want to receive 10 results at most</span>
sc<span class="token punctuation">.</span><span class="token function">setMaxResults</span><span class="token punctuation">(</span><span class="token keyword">new</span> <span class="token class-name">Long</span><span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token class-name">DFAgentDescription</span><span class="token punctuation">[</span><span class="token punctuation">]</span> results <span class="token operator">=</span> <span class="token class-name">DFService</span><span class="token punctuation">.</span><span class="token function">search</span><span class="token punctuation">(</span><span class="token keyword">this</span><span class="token punctuation">,</span> template<span class="token punctuation">,</span> sc<span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token keyword">if</span> <span class="token punctuation">(</span>results<span class="token punctuation">.</span>length <span class="token operator">&gt;</span> <span class="token number">0</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">DFAgentDescription</span> dfd <span class="token operator">=</span> results<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
    <span class="token class-name">AID</span> provider <span class="token operator">=</span> dfd<span class="token punctuation">.</span><span class="token function">getName</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><hr><h2 id="Modelo-de-comunicación" data-id="Modelo-de-comunicación"><a class="anchor hidden-xs" href="#Modelo-de-comunicación" title="Modelo-de-comunicación"><span class="octicon octicon-link"></span></a><span>Modelo de comunicación</span></h2><ul>
<li><span>Basado en el paso de mensajes asíncrono.</span></li>
<li><span>Formato de mensajes definido por el lenguaje ACL (FIPA).</span></li>
</ul><center><img src="https://i.imgur.com/Uh5eZwO.png"></center><h3 id="La-clase-ACLMessage" data-id="La-clase-ACLMessage"><a class="anchor hidden-xs" href="#La-clase-ACLMessage" title="La-clase-ACLMessage"><span class="octicon octicon-link"></span></a><span>La clase ACLMessage</span></h3><ul>
<li><span>Los mensajes intercambiados por los agentes son instancias de la clase </span><code>jade.lang.acl.ACLMessage</code></li>
<li><span>Define métodos de acceso (getters/setters):</span>
<ul>
<li><code>get/setPerformative()</code></li>
<li><code>get/setSender()</code></li>
<li><code>add/getReceiver()</code></li>
<li><code>get/setLanguage()</code></li>
<li><code>get/setOntology</code></li>
<li><code>get/setContent()</code></li>
</ul>
</li>
</ul><h3 id="Envío-y-recepción-de-mensajes" data-id="Envío-y-recepción-de-mensajes"><a class="anchor hidden-xs" href="#Envío-y-recepción-de-mensajes" title="Envío-y-recepción-de-mensajes"><span class="octicon octicon-link"></span></a><span>Envío y recepción de mensajes</span></h3><ul>
<li><span>Enviar un mensaje consiste básicamente en crear un objeto </span><code>ACLMessage</code><span> y llamar al método </span><code>send()</code><span> de </span><code>Agent</code></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token class-name">ACLMessage</span> msg <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">ACLMessage</span><span class="token punctuation">(</span><span class="token class-name">ACLMessage</span><span class="token punctuation">.</span>INFORM<span class="token punctuation">)</span><span class="token punctuation">;</span>
msg<span class="token punctuation">.</span><span class="token function">addReceiver</span><span class="token punctuation">(</span><span class="token keyword">new</span> AID <span class="token punctuation">(</span><span class="token string">"Peter"</span><span class="token punctuation">,</span> AID<span class="token punctuation">.</span>ISLOCALNAME<span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
msg<span class="token punctuation">.</span><span class="token function">setLanguage</span><span class="token punctuation">(</span><span class="token string">"English"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
msg<span class="token punctuation">.</span><span class="token function">setOntology</span><span class="token punctuation">(</span><span class="token string">"Weather-Forecast-Ontology"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
msg<span class="token punctuation">.</span><span class="token function">setContent</span><span class="token punctuation">(</span><span class="token string">"Today it's raining"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token function">send</span><span class="token punctuation">(</span>msg<span class="token punctuation">)</span><span class="token punctuation">;</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><ul>
<li><span>Para procesar mensajes de la cola de mensajes privada, el Agent ejecuta el método </span><code>receive()</code></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token class-name">ACLMessage</span> msg <span class="token operator">=</span> <span class="token function">receive</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
<span class="token keyword">if</span><span class="token punctuation">(</span>msg <span class="token operator">!=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token comment">//Process the message</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><ul>
<li><span>El uso continuo de </span><code>receive()</code><span> es ineficiente.</span></li>
<li><span>Mejor utilizar </span><code>block()</code></li>
<li><span>Permite bloquear el </span><em><span>behaviour</span></em><span> del pool del agente sin bloquear a este.</span></li>
<li><span>Cada vez que llegue un mensaje se desbloquean los </span><em><span>behaviours</span></em><span> bloqueados para que puedan leerlo.</span></li>
<li><span>Método </span><code>blockingReceive()</code><span> disponible (pero peligroso).</span>
<ul>
<li><span>Bloquea todo el agente y no deja que se ejecute ningún otro </span><em><span>behaviour</span></em><span> hasta que llegue el mensaje.</span></li>
</ul>
</li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token keyword">public</span> <span class="token keyword">void</span> <span class="token function">action</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">ACLMessage</span> msg <span class="token operator">=</span> myAgent<span class="token punctuation">.</span><span class="token function">receive</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token keyword">if</span><span class="token punctuation">(</span>msg <span class="token operator">!=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token comment">//Process the message</span>
    <span class="token punctuation">}</span>
    <span class="token keyword">else</span> <span class="token punctuation">{</span>
        <span class="token function">block</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><h3 id="Message-templates" data-id="Message-templates"><a class="anchor hidden-xs" href="#Message-templates" title="Message-templates"><span class="octicon octicon-link"></span></a><span>Message templates</span></h3><ul>
<li><span>Es más seguro hacer uso de </span><em><span>message templates</span></em><span>.</span></li>
</ul><pre style="position: relative;"><code class="java hljs"><div class="wrapper"><div class="gutter linenumber"><span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span>
<span></span></div><div class="code"><span class="token class-name">MessageTemplate</span> tpl <span class="token operator">=</span> <span class="token class-name">MessageTemplate<span class="token punctuation">.</span>MatchOntology</span><span class="token punctuation">(</span><span class="token string">"Test-Ontology"</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

<span class="token keyword">public</span> <span class="token keyword">void</span> <span class="token function">action</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token class-name">ACLMessage</span> msg <span class="token operator">=</span> myAgent<span class="token punctuation">.</span><span class="token function">receive</span><span class="token punctuation">(</span>tlp<span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token keyword">if</span><span class="token punctuation">(</span>msg <span class="token operator">!=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
        <span class="token comment">//Process the message</span>
    <span class="token punctuation">}</span>
    <span class="token keyword">else</span> <span class="token punctuation">{</span>
        <span class="token function">block</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token punctuation">}</span>
<span class="token punctuation">}</span>
</div></div></code><div class="open_grepper_editor" title="Edit &amp; Save To Grepper"></div></pre><ul>
<li><span>Podemos hacer Match con los diferentes elementos de un mensaje:</span>
<ul>
<li><code>Conversation-id</code><span>, </span><code>Ontology</code><span>, </span><code>Language</code><span>, </span><code>Content</code><span>, </span><code>Performative</code></li>
</ul>
</li>
<li><span>Podemos hacer composición mediante </span><code>and</code><span>, </span><code>or</code><span> y </span><code>not</code></li>
</ul><h3 id="Paso-de-mensajes" data-id="Paso-de-mensajes"><a class="anchor hidden-xs" href="#Paso-de-mensajes" title="Paso-de-mensajes"><span class="octicon octicon-link"></span></a><span>Paso de mensajes</span></h3><table>
<thead>
<tr>
<th><span>performative</span></th>
<th><span>passing info</span></th>
<th><span>requesting info</span></th>
<th><span>negotiation</span></th>
<th><span>performing actions</span></th>
<th><span>error handling</span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span>accept-proposal</span></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>agree</span></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>cancel</span></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>cfp</span></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>confirm</span></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>disconfirm</span></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>failure</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
</tr>
<tr>
<td><span>inform</span></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>inform-if</span></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>inform-ref</span></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>not-understood</span></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
</tr>
<tr>
<td><span>propose</span></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>query-if</span></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>query-ref</span></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>refuse</span></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>reject-proposal</span></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
</tr>
<tr>
<td><span>request</span></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>request-when</span></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>request-whenever</span></td>
<td></td>
<td></td>
<td></td>
<td><span>X</span></td>
<td></td>
</tr>
<tr>
<td><span>subscribe</span></td>
<td></td>
<td><span>X</span></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table><h3 id="Protocolos-de-interacción" data-id="Protocolos-de-interacción"><a class="anchor hidden-xs" href="#Protocolos-de-interacción" title="Protocolos-de-interacción"><span class="octicon octicon-link"></span></a><span>Protocolos de interacción</span></h3><p><img src="https://i.imgur.com/xgt4a0K.png" alt="" loading="lazy"></p><ul>
<li><span>Secuencias predefinidas de intercambio de mensajes. En todos ellos se distingue:</span>
<ul>
<li><span>Un </span><strong><span>Initiator</span></strong><span>, que permite gestionar varios Responders a la vez; es un comportamiento que:</span>
<ul>
<li><span>Termina una vez se alcanza un estado final.</span></li>
<li><span>Se puede resetear para reutilizar el objeto (método </span><code>reset()</code><span>).</span></li>
</ul>
</li>
<li><span>Uno o más </span><strong><span>Responder</span></strong><span>, que son implementados por behaviours cíclicos y que vuelven a reintroducirse una vez alcanzan un estado final.</span></li>
</ul>
</li>
<li><strong><span>Referencias</span></strong><span>:</span>
<ul>
<li><span>Capítulo 3.5 de la guía de programación de JADE.</span></li>
<li><span>Documentación de la API (javadoc) de </span><code>jade.proto</code><span>.</span></li>
<li><span>Ejemplos de código en </span><code>examples.protocols</code><span> incluido en la distribución JADE.</span></li>
</ul>
</li>
</ul><h3 id="Soporte-a-los-protocolos-de-interacción" data-id="Soporte-a-los-protocolos-de-interacción"><a class="anchor hidden-xs" href="#Soporte-a-los-protocolos-de-interacción" title="Soporte-a-los-protocolos-de-interacción"><span class="octicon octicon-link"></span></a><span>Soporte a los protocolos de interacción</span></h3><ul>
<li><span>El paquete </span><code>jade.proto</code><span> contiene behaviours para los roles que inician y responden a los protocolos más comunes:</span>
<ul>
<li><span>FIPA-request (AchieveREInitiator/Responder)</span></li>
<li><span>FIPA-Contract-Net (ContractNetInitiator/Responder)</span></li>
<li><span>FIPA-Subscribe (SubscriptionInitiator/Responder)</span></li>
</ul>
</li>
<li><span>Todas estas clases automáticamente se encargan de:</span>
<ul>
<li><span>Comprobar el flujo de mensajes para validar que se corresponde al protocolo.</span></li>
<li><span>De los timeouts (si hay alguno).</span></li>
</ul>
</li>
<li><span>Proveen de métodos de callback que se deben redefinir para tomar las acciones necesarias en los diferentes estados del protocolo; por ejemplo, cuando un mensaje es recibido o expira un timeout.</span></li>
</ul><h3 id="AchieveREInitiatorResponder" data-id="AchieveREInitiatorResponder"><a class="anchor hidden-xs" href="#AchieveREInitiatorResponder" title="AchieveREInitiatorResponder"><span class="octicon octicon-link"></span></a><span>AchieveREInitiator/Responder</span></h3><ul>
<li><span>A lo largo de las últimas versiones JADE se han ido aglutinando los protocolos bajo una misma interfaz: </span><strong><span>AchieveREInitiator/Responder</span></strong><span> o </span><strong><span>SimpleAchieveREInitiator/Responder</span></strong><span> (más rápido pero con menos opciones).</span></li>
<li><span>En general con esta clase podremos iniciar los protocolos más típicos (e.g., Request, Query).</span></li>
<li><span>Al crear una instancia le pasaremos a la constructora el mensaje (</span><code>ACLMessage</code><span>) que queremos enviar: Iniciar el mensaje con el valor correcto de protocolo.</span></li>
<li><span>Podemos iniciarlo con un mensaje incompleto y terminarlo reescribiendo la función </span><code>prepareRequests</code><span>.</span></li>
<li><span>En general podemos extender la clase y sobreescribir las funciones handle… que gestionan los diferentes estados del protocolo (</span><code>refuse</code><span>, </span><code>agree</code><span>, </span><code>response</code><span>).</span></li>
<li><span>Si queremos enviar a varios responders, añadimos a todos en el mensaje. En este caso suele ser útil modificar la función </span><code>handleAllResponses</code><span>, </span><code>handleAllResultNotifications</code><span>.</span></li>
<li><span>En general una vez enviado el mensaje primero recibiremos la primera respuesta (</span><code>agree</code><span>, </span><code>not-understood</code><span>, </span><code>refuse</code><span>) llamando a </span><code>handleResponse</code><span>.</span></li>
<li><span>Y luego, si estaba de acuerdo, el resultado (</span><code>failure</code><span>, </span><code>inform</code><span>).</span></li>
<li><span>En la constructora le pasaremos el template de mensaje sobre el que querremos responder. Normalmente indicaremos el protocolo y la performativa. Podemos usar también </span><code>createMessageTemplate</code><span>.</span></li>
<li><span>Para esta clase podremos reescribir las funciones </span><code>prepare</code><span>… para gestionar los diferentes estados (en especial, </span><code>prepareResponse</code><span> y </span><code>prepareResultNotification</code><span>). Considerad utilizar la función </span><code>createReply</code><span> que se puede llamar mediante la request recibida, así evitamos errores.</span></li>
<li><span>SimpleAchieveREInitiator/Responder:</span>
<ul>
<li><span>Es una versión más compacta y rápida que el protocolo normal.</span></li>
<li><span>No permite registrar behaviours como handlers.</span></li>
<li><span>No permite tener más de un responder.</span></li>
<li><span>Si nuestro protocolo es 1:1 esta sería la mejor opción.</span></li>
<li><span>Podemos igualmente sobreescribir cualquier handler como en el caso anterior.</span></li>
</ul>
</li>
<li><span>Ejemplo sencillo:</span><br>
<img src="https://i.imgur.com/WIUxZzy.png" alt="" loading="lazy"></li>
</ul><h3 id="FIPA-Contract-Net-protocol" data-id="FIPA-Contract-Net-protocol"><a class="anchor hidden-xs" href="#FIPA-Contract-Net-protocol" title="FIPA-Contract-Net-protocol"><span class="octicon octicon-link"></span></a><span>FIPA Contract-Net protocol</span></h3><p><img src="https://i.imgur.com/8E4TY3M.png" alt="" loading="lazy"></p><ul>
<li><span>ContractNetInitiatorAgent</span></li>
<li><span>ContractNetResponderAgent</span></li>
<li><span>Ejecuta los agentes</span>
<ul>
<li><span>Consola</span></li>
<li><span>GUI sniffing</span></li>
<li><span>GUI introspector</span></li>
</ul>
</li>
</ul><hr><h2 id="Gestión-de-contenido" data-id="Gestión-de-contenido"><a class="anchor hidden-xs" href="#Gestión-de-contenido" title="Gestión-de-contenido"><span class="octicon octicon-link"></span></a><span>Gestión de contenido</span></h2><h3 id="ACL-Message" data-id="ACL-Message"><a class="anchor hidden-xs" href="#ACL-Message" title="ACL-Message"><span class="octicon octicon-link"></span></a><span>ACL Message</span></h3><ul>
<li><span>Un ACL Message sigue una estructura fija:</span><br>
<img src="https://i.imgur.com/11IsnIl.png" alt="" loading="lazy"><br>
<img src="https://i.imgur.com/xxOml7w.png" alt="" loading="lazy"></li>
<li><span>ACL: Content:</span>
<ul>
<li><span>En este campo (</span><code>slot</code><span>) está el contenido del mensaje en forma de expresiones.</span></li>
<li><span>La librería de commons-codec se usa para codificar y decodificar estas expresiones que irán en dicho campo.</span>
<ul>
<li><span>En </span><code>jade.content.lang</code><span> encontramos SL y LEAP.</span></li>
<li><span>Estas codifican las expresiones según el estándar especificado FIPA-SL y FIPA-LEAP. El primero es más legible.</span></li>
<li><span>Podríamos especificar otros codecs (XML, RDF, OWL).</span></li>
</ul>
</li>
</ul>
</li>
</ul><h3 id="Content-Manager" data-id="Content-Manager"><a class="anchor hidden-xs" href="#Content-Manager" title="Content-Manager"><span class="octicon octicon-link"></span></a><span>Content Manager</span></h3><p><span>JADE, a través del Content Manager:</span></p><ul>
<li><span>Permite la codificación/decodificación del contenido de los mensajes (usando los codecs).</span></li>
<li><span>Verifica que sean correctos (formatos, tipos) (usando la ontología).</span></li>
<li><span>Como para los agentes JADE la manipulación es más cómoda con objetos Java que con Strings, requiere que la ontología este en ese formato.</span></li>
<li><span>Básicamente serializa en un formato y lo deserializa. Al hacer esto último crea las instancias al reificar.</span></li>
<li><span>Podríamos hacer agentes que manipulan los mensajes de una manera más compleja (AgentOWL).</span></li>
</ul><h3 id="Ontología-para-JADE" data-id="Ontología-para-JADE"><a class="anchor hidden-xs" href="#Ontología-para-JADE" title="Ontología-para-JADE"><span class="octicon octicon-link"></span></a><span>Ontología para JADE</span></h3><ul>
<li><span>Necesitamos una ontología:</span>
<ul>
<li><span>Definición de elementos de la ontología.</span></li>
<li><span>Definición de las clases Java correspondiente.</span></li>
</ul>
</li>
<li><span>Podríamos hacernos la ontología mediante clases Java tal y como define JADE (es decir, siguiendo sus convenciones)</span>
<ul>
<li><span>Mirad en referencias (al final de las slides) - Tutorial.</span></li>
</ul>
</li>
<li><span>Para facilitarnos la vida podemos usar un plugin para Protégé que nos permitirá transformar una ontología en las clases Java para JADE.</span>
<ul>
<li><a href="https://protegewiki.stanford.edu/wiki/OntologyBeanGenerator" target="_blank" rel="noopener"><span>https://protegewiki.stanford.edu/wiki/OntologyBeanGenerator</span></a></li>
<li><span>Necesitaremos una versión antigua de Protégé (3.4)</span></li>
</ul>
</li>
<li><strong><span>Usando la ontología</span></strong><span>:</span>
<ol>
<li><span>Nos importaremos el código generado al proyecto.</span></li>
<li><span>Crearemos instancias usando las clases (tanto para conceptos como propiedades).</span></li>
<li><span>En el setup del agente registraremos en este el lenguaje y ontología. </span><img src="https://i.imgur.com/PTdSn0Y.png" alt="" loading="lazy"></li>
<li><span>Crearemos el ACLMessage donde indicaremos la ontología.</span><img src="https://i.imgur.com/MDVYnPN.png" alt="" loading="lazy"></li>
<li><span>Mediante </span><code>myAgent.getContentManager.fillContent</code><span> añadiremos al mensaje creado las instancias.</span><img src="https://i.imgur.com/MCmjy0G.png" alt="" loading="lazy"></li>
<li><span>En el receptor, utilizaremos la función </span><code>getContentManager().extractContent(msg)</code><span>. Después podemos comprobar con </span><code>instanceOf</code><span> de que clase son las cosas (si hiciera falta).</span></li>
<li><span>En general utilizaríamos algún lenguaje de contenido como FIPA-SL para construir expresiones indicando si, por ejemplo, tenemos alguna cosa, si no tenemos esa cosa, si podemos descargar, etc…</span>
<ul>
<li><span>Por ejemplo, para indicar que una persona no trabaja en X: </span><img src="https://i.imgur.com/t0VLkOX.png" alt="" loading="lazy"></li>
</ul>
</li>
<li><span>Ojo, para las acciones (como descargar) tenemos que crear un objeto </span><code>Action</code><span> y después definir el actor y la acción concreta (</span><code>setActor</code><span> y </span><code>setAction</code><span>). Ese será el contenido del mensaje.</span></li>
</ol>
</li>
<li><strong><span>Referencias:</span></strong>
<ul>
<li><span>Tutorial: APPLICATION-DEFINED CONTENT LANGUAGES AND ONTOLOGIES: </span><a href="http://jade.tilab.com/doc/tutorials/CLOntoSupport.pdf" target="_blank" rel="noopener"><span>http://jade.tilab.com/doc/tutorials/CLOntoSupport.pdf</span></a></li>
</ul>
</li>
</ul></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
<li class=""><a href="#Introducción-a-JADE" title="Introducción a JADE">Introducción a JADE</a><ul class="nav">
<li class=""><a href="#Setup-del-entorno" title="Setup del entorno">Setup del entorno</a></li>
<li class=""><a href="#Agentes" title="Agentes">Agentes</a><ul class="nav">
<li class=""><a href="#Nombres-locales-GUID-y-direcciones" title="Nombres locales, GUID y direcciones">Nombres locales, GUID y direcciones</a></li>
<li class=""><a href="#Paso-de-parámetros" title="Paso de parámetros">Paso de parámetros</a></li>
<li class=""><a href="#Expiración-del-agente" title="Expiración del agente">Expiración del agente</a></li>
<li class=""><a href="#Construyendo-un-agente" title="Construyendo un agente">Construyendo un agente</a></li>
<li class=""><a href="#Ciclo-de-vida-del-agente" title="Ciclo de vida del agente">Ciclo de vida del agente</a></li>
<li class=""><a href="#Estados-del-agente" title="Estados del agente">Estados del agente</a></li>
</ul>
</li>
<li class=""><a href="#Comportamientos-Behaviours" title="Comportamientos (Behaviours)">Comportamientos (Behaviours)</a><ul class="nav">
<li class=""><a href="#Planificación-y-ejecución-de-Behaviours" title="Planificación y ejecución de Behaviours">Planificación y ejecución de Behaviours</a></li>
<li class=""><a href="#Tipos-de-Behaviours" title="Tipos de Behaviours">Tipos de Behaviours</a></li>
<li class=""><a href="#Empezar-y-acabar-los-Behaviours" title="Empezar y acabar los Behaviours">Empezar y acabar los Behaviours</a></li>
</ul>
</li>
<li class=""><a href="#Directory-Facilitator-DF" title="Directory Facilitator (DF)">Directory Facilitator (DF)</a><ul class="nav">
<li class=""><a href="#Registro" title="Registro">Registro</a></li>
<li class=""><a href="#Búsqueda" title="Búsqueda">Búsqueda</a></li>
</ul>
</li>
<li class=""><a href="#Modelo-de-comunicación" title="Modelo de comunicación">Modelo de comunicación</a><ul class="nav">
<li class=""><a href="#La-clase-ACLMessage" title="La clase ACLMessage">La clase ACLMessage</a></li>
<li class=""><a href="#Envío-y-recepción-de-mensajes" title="Envío y recepción de mensajes">Envío y recepción de mensajes</a></li>
<li class=""><a href="#Message-templates" title="Message templates">Message templates</a></li>
<li class=""><a href="#Paso-de-mensajes" title="Paso de mensajes">Paso de mensajes</a></li>
<li class=""><a href="#Protocolos-de-interacción" title="Protocolos de interacción">Protocolos de interacción</a></li>
<li class=""><a href="#Soporte-a-los-protocolos-de-interacción" title="Soporte a los protocolos de interacción">Soporte a los protocolos de interacción</a></li>
<li class=""><a href="#AchieveREInitiatorResponder" title="AchieveREInitiator/Responder">AchieveREInitiator/Responder</a></li>
<li class=""><a href="#FIPA-Contract-Net-protocol" title="FIPA Contract-Net protocol">FIPA Contract-Net protocol</a></li>
</ul>
</li>
<li class=""><a href="#Gestión-de-contenido" title="Gestión de contenido">Gestión de contenido</a><ul class="nav">
<li class=""><a href="#ACL-Message" title="ACL Message">ACL Message</a></li>
<li class=""><a href="#Content-Manager" title="Content Manager">Content Manager</a></li>
<li class=""><a href="#Ontología-para-JADE" title="Ontología para JADE">Ontología para JADE</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
            </ul>
        </div>
    </div>
    <div id="ui-toc-affix" class="ui-affix-toc ui-toc-dropdown unselectable hidden-print" data-spy="affix" style="top:17px;display:none;" null null>
        <div class="toc"><ul class="nav">
<li class=""><a href="#Introducción-a-JADE" title="Introducción a JADE">Introducción a JADE</a><ul class="nav">
<li class=""><a href="#Setup-del-entorno" title="Setup del entorno">Setup del entorno</a></li>
<li class=""><a href="#Agentes" title="Agentes">Agentes</a><ul class="nav">
<li class=""><a href="#Nombres-locales-GUID-y-direcciones" title="Nombres locales, GUID y direcciones">Nombres locales, GUID y direcciones</a></li>
<li class=""><a href="#Paso-de-parámetros" title="Paso de parámetros">Paso de parámetros</a></li>
<li class=""><a href="#Expiración-del-agente" title="Expiración del agente">Expiración del agente</a></li>
<li class=""><a href="#Construyendo-un-agente" title="Construyendo un agente">Construyendo un agente</a></li>
<li class=""><a href="#Ciclo-de-vida-del-agente" title="Ciclo de vida del agente">Ciclo de vida del agente</a></li>
<li class=""><a href="#Estados-del-agente" title="Estados del agente">Estados del agente</a></li>
</ul>
</li>
<li class=""><a href="#Comportamientos-Behaviours" title="Comportamientos (Behaviours)">Comportamientos (Behaviours)</a><ul class="nav">
<li class=""><a href="#Planificación-y-ejecución-de-Behaviours" title="Planificación y ejecución de Behaviours">Planificación y ejecución de Behaviours</a></li>
<li class=""><a href="#Tipos-de-Behaviours" title="Tipos de Behaviours">Tipos de Behaviours</a></li>
<li class=""><a href="#Empezar-y-acabar-los-Behaviours" title="Empezar y acabar los Behaviours">Empezar y acabar los Behaviours</a></li>
</ul>
</li>
<li class=""><a href="#Directory-Facilitator-DF" title="Directory Facilitator (DF)">Directory Facilitator (DF)</a><ul class="nav">
<li class=""><a href="#Registro" title="Registro">Registro</a></li>
<li class=""><a href="#Búsqueda" title="Búsqueda">Búsqueda</a></li>
</ul>
</li>
<li class=""><a href="#Modelo-de-comunicación" title="Modelo de comunicación">Modelo de comunicación</a><ul class="nav">
<li class=""><a href="#La-clase-ACLMessage" title="La clase ACLMessage">La clase ACLMessage</a></li>
<li class=""><a href="#Envío-y-recepción-de-mensajes" title="Envío y recepción de mensajes">Envío y recepción de mensajes</a></li>
<li class=""><a href="#Message-templates" title="Message templates">Message templates</a></li>
<li class=""><a href="#Paso-de-mensajes" title="Paso de mensajes">Paso de mensajes</a></li>
<li class=""><a href="#Protocolos-de-interacción" title="Protocolos de interacción">Protocolos de interacción</a></li>
<li class=""><a href="#Soporte-a-los-protocolos-de-interacción" title="Soporte a los protocolos de interacción">Soporte a los protocolos de interacción</a></li>
<li class=""><a href="#AchieveREInitiatorResponder" title="AchieveREInitiator/Responder">AchieveREInitiator/Responder</a></li>
<li class=""><a href="#FIPA-Contract-Net-protocol" title="FIPA Contract-Net protocol">FIPA Contract-Net protocol</a></li>
</ul>
</li>
<li class=""><a href="#Gestión-de-contenido" title="Gestión de contenido">Gestión de contenido</a><ul class="nav">
<li class=""><a href="#ACL-Message" title="ACL Message">ACL Message</a></li>
<li class=""><a href="#Content-Manager" title="Content Manager">Content Manager</a></li>
<li class=""><a href="#Ontología-para-JADE" title="Ontología para JADE">Ontología para JADE</a></li>
</ul>
</li>
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
