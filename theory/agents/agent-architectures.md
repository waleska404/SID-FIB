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
        Agent Architectures - HackMD
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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Agent-Architectures" data-id="Agent-Architectures"><a class="anchor hidden-xs" href="#Agent-Architectures" title="Agent-Architectures"><span class="octicon octicon-link"></span></a><span>Agent Architectures</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Agent-Architectures" title="Agent Architectures">Agent Architectures</a><ul>
<li><a href="#Abstract-Architecture-for-Agents" title="Abstract Architecture for Agents">Abstract Architecture for Agents</a><ul>
<li><a href="#Reactive-Agents" title="Reactive Agents">Reactive Agents</a></li>
<li><a href="#Purely-Reactive-Agents" title="Purely Reactive Agents">Purely Reactive Agents</a></li>
<li><a href="#Reactive-Agents-with-Internal-State" title="Reactive Agents with Internal State">Reactive Agents with Internal State</a></li>
<li><a href="#AdvantagesDisadvantages-of-Reactive-Agents" title="Advantages/Disadvantages of Reactive Agents">Advantages/Disadvantages of Reactive Agents</a></li>
<li><a href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated Automata Components: RULER and GAPPS">Situated Automata Components: RULER and GAPPS</a></li>
<li><a href="#Delliberative-Agents-with-expected-utilities" title="Delliberative Agents (with expected utilities)">Delliberative Agents (with expected utilities)</a></li>
<li><a href="#Delliberative-Agents-with-explicit-goals" title="Delliberative Agents (with explicit goals)">Delliberative Agents (with explicit goals)</a></li>
<li><a href="#Agents’-Interactions" title="Agents’ Interactions">Agents’ Interactions</a></li>
</ul>
</li>
<li><a href="#Architectures-for-Multiagent-Systems" title="Architectures for Multiagent Systems">Architectures for Multiagent Systems</a><ul>
<li><a href="#MAS---many-agents-in-the-same-environment" title="MAS - many agents in the same environment">MAS - many agents in the same environment</a></li>
<li><a href="#Agent-Platform" title="Agent Platform">Agent Platform</a></li>
<li><a href="#Components-of-an-Agent-Platform" title="Components of an Agent Platform">Components of an Agent Platform</a></li>
<li><a href="#Communication-methods" title="Communication methods">Communication methods</a></li>
<li><a href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA Architecture for Agent Platforms">FIPA Architecture for Agent Platforms</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Abstract-Architecture-for-Agents" data-id="Abstract-Architecture-for-Agents"><a class="anchor hidden-xs" href="#Abstract-Architecture-for-Agents" title="Abstract-Architecture-for-Agents"><span class="octicon octicon-link"></span></a><span>Abstract Architecture for Agents</span></h2><ul>
<li><span>An </span><u><span>agent architecture</span></u><span> proposes a particular </span><strong><span>methodology for building an autonomous agent.</span></strong></li>
<li><span>How the construction of the agent can be decomposed into the construction of a set of </span><strong><span>component modules</span></strong><span>.</span>
<ul>
<li><span>How these modules should be made to </span><strong><span>interact</span></strong><span>.</span></li>
</ul>
</li>
<li><span>These two aspects define how the </span><strong><span>sensor data</span></strong><span> and the </span><strong><span>current internal state</span></strong><span> of the agent determine the </span><strong><span>actions</span></strong><span> (effector outputs) and future internal state of the agent.</span></li>
</ul><h3 id="Reactive-Agents" data-id="Reactive-Agents"><a class="anchor hidden-xs" href="#Reactive-Agents" title="Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Reactive Agents</span></h3><ul>
<li><span>Simple processing units that perceive and react to changes in their environment.</span></li>
<li><span>Do not have a symbolic representation of the world and do not use complex symbolic reasoning.</span></li>
<li><span>The advocates of reactive agent systems claims that intelligence is not a property of the active entity but it is distributed in the system, and steams as the result of the interaction between the many entities of the distributed structure and the environment.</span></li>
</ul><h3 id="Purely-Reactive-Agents" data-id="Purely-Reactive-Agents"><a class="anchor hidden-xs" href="#Purely-Reactive-Agents" title="Purely-Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Purely Reactive Agents</span></h3><ul>
<li><u><span>Purely reactive agents</span></u><span>: agents that decide what to do without reference to their  history — they </span><strong><span>base their decision making entirely on the present</span></strong><span>, with no reference at all to the past.</span></li>
</ul><p><img src="https://i.imgur.com/YYHyeTI.png" alt="" loading="lazy"></p><p><img src="https://i.imgur.com/oBybAvZ.png" alt="" loading="lazy"></p><h3 id="Reactive-Agents-with-Internal-State" data-id="Reactive-Agents-with-Internal-State"><a class="anchor hidden-xs" href="#Reactive-Agents-with-Internal-State" title="Reactive-Agents-with-Internal-State"><span class="octicon octicon-link"></span></a><span>Reactive Agents with Internal State</span></h3><p><img src="https://i.imgur.com/BEakQz9.png" alt="" loading="lazy"></p><p><img src="https://i.imgur.com/R0AQ4X6.png" alt="" loading="lazy"></p><h3 id="AdvantagesDisadvantages-of-Reactive-Agents" data-id="AdvantagesDisadvantages-of-Reactive-Agents"><a class="anchor hidden-xs" href="#AdvantagesDisadvantages-of-Reactive-Agents" title="AdvantagesDisadvantages-of-Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Advantages/Disadvantages of Reactive Agents</span></h3><ul>
<li>
<p><u><span>Advantages:</span></u></p>
<ul>
<li><strong><span>Simplicity</span></strong><span> of individual agents.</span></li>
<li><strong><span>Flexibility</span></strong><span>, adaptability: Ideal in very dynamic and unpredictable environments.</span></li>
<li><strong><span>Computational tractability</span></strong><span>: Avoiding complex planning/reasoning. Avoiding continuous model update.</span></li>
<li><strong><span>Robustness</span></strong><span> against failure: No central planning component (e.g. ant colony).</span></li>
<li><strong><span>Elegance</span></strong><span>.</span></li>
</ul>
</li>
<li>
<p><u><span>Disadvantages:</span></u></p>
<ul>
<li><strong><span>Need for sufficient information</span></strong><span> from the local environment.</span></li>
<li><span>Unclear how to incorporate </span><strong><span>non-local information</span></strong><span>.</span></li>
<li><strong><span>No long-term planning</span></strong><span> or replanning capabilities.</span></li>
<li><strong><span>Applicability is limited</span></strong><span>.</span></li>
<li><span>Difficult to make reactive agents that </span><strong><span>learn</span></strong><span>.</span></li>
<li><span>Interactions with the environment can have </span><strong><span>unpredictable long-term consequences</span></strong><span>. Dynamics of interaction can become too complex to understand.</span></li>
</ul>
</li>
</ul><h3 id="Situated-Automata-Components-RULER-and-GAPPS" data-id="Situated-Automata-Components-RULER-and-GAPPS"><a class="anchor hidden-xs" href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated-Automata-Components-RULER-and-GAPPS"><span class="octicon octicon-link"></span></a><span>Situated Automata Components: RULER and GAPPS</span></h3><ul>
<li>
<p><span>An agent is specified in terms of two components: </span><strong><span>perception</span></strong><span> and </span><strong><span>action</span></strong><span>. Two programs are then used to synthesize agents:</span></p>
<ul>
<li><strong><span>RULER</span></strong><span> is used to specify the </span><u><span>perception component</span></u><span> of an agent.</span></li>
<li><strong><span>GAPPS</span></strong><span> is used to specify the </span><u><span>action component</span></u><span>.</span></li>
</ul>
</li>
<li>
<p><strong><u><span>RULER</span></u><span>:</span></strong></p>
<ul>
<li><span>RULER takes as its input three components:</span><br>
<strong><span>1.</span></strong><span> The </span><strong><span>semantics</span></strong><span> of the agent’s inputs (‘whenever bit 1 is on, it is raining’).</span><br>
<strong><span>2.</span></strong><span> A set of </span><strong><span>static facts</span></strong><span> (‘whenever it is raining, the ground is wet’).</span><br>
<strong><span>3.</span></strong><span> A specification of the </span><strong><span>state transitions of the world</span></strong><span> (‘if the ground is wet, it stays wet until the sun comes out’).</span></li>
<li><span>The programmer then specifies the </span><u><span>desired semantics for the output</span></u><span> (‘if this bit is on, the ground is wet’).</span></li>
<li><span>The compiler designs a circuit whose output will have the correct semantics.</span></li>
</ul>
</li>
<li>
<p><strong><u><span>GAPPS</span></u><span>:</span></strong></p>
<ul>
<li><span>GAPPS program takes as its input:</span><br>
<strong><span>1.</span></strong><span> A set of </span><strong><span>goal reduction rules</span></strong><span>: Rules that encode information about how goals can be achieved in a given state.</span><br>
<strong><span>2.</span></strong><span> A </span><strong><span>top level goal</span></strong><span>.</span></li>
<li><span>Then it generates a program that can be translated into a digital circuit in order to realize the goal.</span></li>
<li><span>The generated circuit does not represent or manipulate symbolic expressions; all symbolic manipulation is done at compile time.</span></li>
</ul>
</li>
</ul><h4 id="From-perception-to-action" data-id="From-perception-to-action"><a class="anchor hidden-xs" href="#From-perception-to-action" title="From-perception-to-action"><span class="octicon octicon-link"></span></a><span>From perception to action</span></h4><p><img src="https://i.imgur.com/VAUpV0G.png" alt="" loading="lazy"></p><h3 id="Delliberative-Agents-with-expected-utilities" data-id="Delliberative-Agents-with-expected-utilities"><a class="anchor hidden-xs" href="#Delliberative-Agents-with-expected-utilities" title="Delliberative-Agents-with-expected-utilities"><span class="octicon octicon-link"></span></a><span>Delliberative Agents (with expected utilities)</span></h3><ul>
<li><span>We build agents in order to carry out tasks for us. The task must be specified by us… But we want to </span><strong><span>tell agents what to do without telling them how to do it</span></strong><span>.</span></li>
<li><span>One possibility: </span><strong><span>associate utilities with individual states</span></strong><span> — the task of the agent is then to bring about states that maximize utility.</span></li>
<li><strong><u><span>Utility Functions over States</span></u><span>:</span></strong>
<ul>
<li><span>A task specification is a function </span><code>u : E → #</code><span> which associates a </span><strong><span>real number with every environment state</span></strong><span>.</span></li>
<li><span>But what is the value of a </span><strong><span>run</span></strong><span>…</span>
<ul>
<li><span>minimum utility of state on run?</span></li>
<li><span>maximum utility of state on run?</span></li>
<li><span>sum of utilities of states on run?</span></li>
<li><span>average?</span></li>
</ul>
</li>
<li><strong><span>Disadvantage</span></strong><span>: difficult to specify a </span><strong><span>long term</span></strong><span> view when assigning utilities to individual states (One possibility: a </span><strong><span>discount</span></strong><span> for states later on).</span></li>
</ul>
</li>
<li><strong><u><span>Utilities over Runs</span></u><span>:</span></strong>
<ul>
<li><span>Another possibility: </span><code>u : R → #</code><span> </span><strong><span>assigning a utilities to a runs</span></strong><span>, instead of assigning them to individual states.</span></li>
<li><span>Such an approach takes an inherently </span><strong><span>long term view</span></strong><span>.</span></li>
<li><span>Other variations: incorporate probabilities of different states emerging.</span></li>
<li><strong><span>Difficulties</span></strong><span> with utility-based approaches:</span>
<ul>
<li><span>where do the numbers come from?</span></li>
<li><span>we (normally?) do not think in terms of utilities!</span></li>
<li><span>hard to formulate tasks in these terms.</span></li>
</ul>
</li>
</ul>
</li>
</ul><p><img src="https://i.imgur.com/IMrkKWT.png" alt="" loading="lazy"></p><h3 id="Delliberative-Agents-with-explicit-goals" data-id="Delliberative-Agents-with-explicit-goals"><a class="anchor hidden-xs" href="#Delliberative-Agents-with-explicit-goals" title="Delliberative-Agents-with-explicit-goals"><span class="octicon octicon-link"></span></a><span>Delliberative Agents (with explicit goals)</span></h3><p><img src="https://i.imgur.com/OtjVpz8.png" alt="" loading="lazy"><br>
<img src="https://i.imgur.com/LG91tuG.png" alt="" loading="lazy"></p><h3 id="Agents’-Interactions" data-id="Agents’-Interactions"><a class="anchor hidden-xs" href="#Agents’-Interactions" title="Agents’-Interactions"><span class="octicon octicon-link"></span></a><span>Agents’ Interactions</span></h3><ul>
<li><span>Interaction between agents is </span><strong><span>unavoidable</span></strong><span>.</span>
<ul>
<li><span>To achieve </span><strong><span>own goals</span></strong><span>.</span></li>
<li><span>To manage </span><strong><span>interdependencies</span></strong><span>.</span></li>
</ul>
</li>
<li><span>It should occur at </span><strong><span>Knowledge-level</span></strong><span>.</span>
<ul>
<li><span>Which goals?, When?, Who executes what?</span></li>
</ul>
</li>
<li><strong><span>Flexibility</span></strong><span> to start and to give answers.</span>
<ul>
<li><strong><span>Asynchronous</span></strong><span> communication.</span></li>
<li><span>Need for </span><strong><span>languages and protocols</span></strong><span>.</span></li>
</ul>
</li>
</ul><blockquote style="border-left-color: rgb(255, 0, 0);">
<p><span>This implies a radical change in the way programs usually interact.</span><span class="color" data-color="#ff0000"></span></p>
</blockquote><hr><h2 id="Architectures-for-Multiagent-Systems" data-id="Architectures-for-Multiagent-Systems"><a class="anchor hidden-xs" href="#Architectures-for-Multiagent-Systems" title="Architectures-for-Multiagent-Systems"><span class="octicon octicon-link"></span></a><span>Architectures for Multiagent Systems</span></h2><h3 id="MAS---many-agents-in-the-same-environment" data-id="MAS---many-agents-in-the-same-environment"><a class="anchor hidden-xs" href="#MAS---many-agents-in-the-same-environment" title="MAS---many-agents-in-the-same-environment"><span class="octicon octicon-link"></span></a><span>MAS - many agents in the same environment</span></h3><p><span>Interactions among agents. Interactions for: High-level interactions, Coordination, Communication and Organization.</span></p><ul>
<li><strong><span>Coordination</span></strong>
<ul>
<li><span>Collectively motivated / interested</span>
<ul>
<li><span>own goals / coalition</span></li>
</ul>
</li>
<li><span>Self interested</span>
<ul>
<li><span>own goals / indifferent</span></li>
<li><span>own goals / competition / competing for the same resources</span></li>
<li><span>own goals / competition / contradictory goals</span></li>
</ul>
</li>
</ul>
</li>
<li><strong><span>Communication</span></strong>
<ul>
<li><span>Communication protocol</span>
<ul>
<li><span>negotiation to reach agreement</span></li>
</ul>
</li>
<li><span>Communication language</span>
<ul>
<li><span>ontologies</span></li>
</ul>
</li>
</ul>
</li>
<li><strong><span>Organizational structures</span></strong>
<ul>
<li><span>centralized vs decentralized</span></li>
<li><span>hierarchical/markets</span></li>
</ul>
</li>
</ul><p><img src="https://i.imgur.com/edwe58W.png" alt="" loading="lazy"></p><h3 id="Agent-Platform" data-id="Agent-Platform"><a class="anchor hidden-xs" href="#Agent-Platform" title="Agent-Platform"><span class="octicon octicon-link"></span></a><span>Agent Platform</span></h3><ul>
<li><span>Agents in a multiagent system tend to interact through a </span><strong><span>middleware layer</span></strong><span>.</span></li>
<li><span>This middleware provides connectivity between agents, solving low-level connectivity issues: Communication methods.</span></li>
<li><span>Sometimes this middleware is called </span><strong><span>agent platform</span></strong><span>.</span></li>
<li><span>Agent Platform </span><strong><span>tasks</span></strong><span>:</span>
<ul>
<li><span>Suspend temporally an agent execution</span></li>
<li><span>Stop an agent execution.</span></li>
<li><span>Resume/continue agent execution.</span></li>
<li><span>Start an agent.</span></li>
<li><span>Platform resource management.</span></li>
</ul>
</li>
</ul><h3 id="Components-of-an-Agent-Platform" data-id="Components-of-an-Agent-Platform"><a class="anchor hidden-xs" href="#Components-of-an-Agent-Platform" title="Components-of-an-Agent-Platform"><span class="octicon octicon-link"></span></a><span>Components of an Agent Platform</span></h3><ul>
<li><strong><span>Agent</span></strong><span>: a program providing a list of services.</span></li>
<li><strong><span>Directory Facilitator (DF)</span></strong><span> is an agent which provides a Yellow Pages service within the platform </span><u><span>(knows the services that agents within the platform provide)</span></u><span>.</span>
<ul>
<li><u><span>register, deregister, modify, search</span></u></li>
</ul>
</li>
<li><strong><span>Agent Management System (AMS)</span></strong><span> is an agent controlling access and usage of the agent platform. It knows the platform and agents’ </span><strong><span>addresses</span></strong><span> and provides a White Pages service (knows the routing addresses for agents within and in other platforms).</span></li>
<li><strong><span>Message Transport Service (MTS)</span></strong><span> is used to enable communication between agents in different platforms.</span></li>
</ul><h3 id="Communication-methods" data-id="Communication-methods"><a class="anchor hidden-xs" href="#Communication-methods" title="Communication-methods"><span class="octicon octicon-link"></span></a><span>Communication methods</span></h3><ul>
<li><strong><span>Blackboard systems</span></strong>
<ul>
<li><span>Agents communicate information through a common data structure, accessible by everybody.</span></li>
<li><span>Problem: if there is no middleware to provide some concurrency, it tends to become a bottleneck.</span></li>
</ul>
</li>
<li><strong><span>Message passing</span></strong>
<ul>
<li><span>Agents communicate directly by means of messages.</span></li>
<li><span>The agent platform usually acts as message router.</span></li>
<li><span>Common communication language (e.g. </span><strong><span>FIPA-ACL</span></strong><span>).</span></li>
<li><span>Common communication protocols (message format, steps in a communication).</span></li>
</ul>
</li>
</ul><h3 id="FIPA-Architecture-for-Agent-Platforms" data-id="FIPA-Architecture-for-Agent-Platforms"><a class="anchor hidden-xs" href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA-Architecture-for-Agent-Platforms"><span class="octicon octicon-link"></span></a><span>FIPA Architecture for Agent Platforms</span></h3><p><img src="https://i.imgur.com/l5mj9wY.png" alt="" loading="lazy"></p></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
<li class=""><a href="#Agent-Architectures" title="Agent Architectures">Agent Architectures</a><ul class="nav">
<li class=""><a href="#Abstract-Architecture-for-Agents" title="Abstract Architecture for Agents">Abstract Architecture for Agents</a><ul class="nav">
<li class=""><a href="#Reactive-Agents" title="Reactive Agents">Reactive Agents</a></li>
<li class=""><a href="#Purely-Reactive-Agents" title="Purely Reactive Agents">Purely Reactive Agents</a></li>
<li class=""><a href="#Reactive-Agents-with-Internal-State" title="Reactive Agents with Internal State">Reactive Agents with Internal State</a></li>
<li class=""><a href="#AdvantagesDisadvantages-of-Reactive-Agents" title="Advantages/Disadvantages of Reactive Agents">Advantages/Disadvantages of Reactive Agents</a></li>
<li class=""><a href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated Automata Components: RULER and GAPPS">Situated Automata Components: RULER and GAPPS</a></li>
<li class=""><a href="#Delliberative-Agents-with-expected-utilities" title="Delliberative Agents (with expected utilities)">Delliberative Agents (with expected utilities)</a></li>
<li class=""><a href="#Delliberative-Agents-with-explicit-goals" title="Delliberative Agents (with explicit goals)">Delliberative Agents (with explicit goals)</a></li>
<li class=""><a href="#Agents’-Interactions" title="Agents’ Interactions">Agents’ Interactions</a></li>
</ul>
</li>
<li class=""><a href="#Architectures-for-Multiagent-Systems" title="Architectures for Multiagent Systems">Architectures for Multiagent Systems</a><ul class="nav">
<li class=""><a href="#MAS---many-agents-in-the-same-environment" title="MAS - many agents in the same environment">MAS - many agents in the same environment</a></li>
<li class=""><a href="#Agent-Platform" title="Agent Platform">Agent Platform</a></li>
<li class=""><a href="#Components-of-an-Agent-Platform" title="Components of an Agent Platform">Components of an Agent Platform</a></li>
<li class=""><a href="#Communication-methods" title="Communication methods">Communication methods</a></li>
<li class=""><a href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA Architecture for Agent Platforms">FIPA Architecture for Agent Platforms</a></li>
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
<li class=""><a href="#Agent-Architectures" title="Agent Architectures">Agent Architectures</a><ul class="nav">
<li class=""><a href="#Abstract-Architecture-for-Agents" title="Abstract Architecture for Agents">Abstract Architecture for Agents</a><ul class="nav">
<li class=""><a href="#Reactive-Agents" title="Reactive Agents">Reactive Agents</a></li>
<li class=""><a href="#Purely-Reactive-Agents" title="Purely Reactive Agents">Purely Reactive Agents</a></li>
<li class=""><a href="#Reactive-Agents-with-Internal-State" title="Reactive Agents with Internal State">Reactive Agents with Internal State</a></li>
<li class=""><a href="#AdvantagesDisadvantages-of-Reactive-Agents" title="Advantages/Disadvantages of Reactive Agents">Advantages/Disadvantages of Reactive Agents</a></li>
<li class=""><a href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated Automata Components: RULER and GAPPS">Situated Automata Components: RULER and GAPPS</a></li>
<li class=""><a href="#Delliberative-Agents-with-expected-utilities" title="Delliberative Agents (with expected utilities)">Delliberative Agents (with expected utilities)</a></li>
<li class=""><a href="#Delliberative-Agents-with-explicit-goals" title="Delliberative Agents (with explicit goals)">Delliberative Agents (with explicit goals)</a></li>
<li class=""><a href="#Agents’-Interactions" title="Agents’ Interactions">Agents’ Interactions</a></li>
</ul>
</li>
<li class=""><a href="#Architectures-for-Multiagent-Systems" title="Architectures for Multiagent Systems">Architectures for Multiagent Systems</a><ul class="nav">
<li class=""><a href="#MAS---many-agents-in-the-same-environment" title="MAS - many agents in the same environment">MAS - many agents in the same environment</a></li>
<li class=""><a href="#Agent-Platform" title="Agent Platform">Agent Platform</a></li>
<li class=""><a href="#Components-of-an-Agent-Platform" title="Components of an Agent Platform">Components of an Agent Platform</a></li>
<li class=""><a href="#Communication-methods" title="Communication methods">Communication methods</a></li>
<li class=""><a href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA Architecture for Agent Platforms">FIPA Architecture for Agent Platforms</a></li>
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
