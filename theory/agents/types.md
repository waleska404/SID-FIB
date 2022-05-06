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
        Agent Types and Architectures - HackMD
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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Agent-Types-and-Architectures" data-id="Agent-Types-and-Architectures"><a class="anchor hidden-xs" href="#Agent-Types-and-Architectures" title="Agent-Types-and-Architectures"><span class="octicon octicon-link"></span></a><span>Agent Types and Architectures</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Agent-Types-and-Architectures" title="Agent Types and Architectures">Agent Types and Architectures</a><ul>
<li><a href="#Agent-Properties" title="Agent Properties">Agent Properties</a><ul>
<li><a href="#Agent-Definitions" title="Agent Definitions">Agent Definitions</a></li>
<li><a href="#Autonomy" title="Autonomy">Autonomy</a></li>
<li><a href="#Flexibility" title="Flexibility">Flexibility</a></li>
<li><a href="#Reactivity" title="Reactivity">Reactivity</a></li>
<li><a href="#Proactivness" title="Proactivness">Proactivness</a></li>
<li><a href="#Social-Ability" title="Social Ability">Social Ability</a></li>
<li><a href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing Reactive and Goal-Oriented Behaviour">Balancing Reactive and Goal-Oriented Behaviour</a></li>
<li><a href="#Other" title="Other">Other</a></li>
</ul>
</li>
<li><a href="#Environment-Properties" title="Environment Properties">Environment Properties</a><ul>
<li><a href="#Accessible-vs-Inaccessible" title="Accessible vs. Inaccessible">Accessible vs. Inaccessible</a></li>
<li><a href="#Deterministic-vs-non-Deterministic" title="Deterministic vs. non-Deterministic">Deterministic vs. non-Deterministic</a></li>
<li><a href="#Episodic-vs-non-Episodic" title="Episodic vs. non-Episodic">Episodic vs. non-Episodic</a></li>
<li><a href="#Static-vs-Dynamic" title="Static vs. Dynamic">Static vs. Dynamic</a></li>
<li><a href="#Discrete-vs-Continuous" title="Discrete vs. Continuous">Discrete vs. Continuous</a></li>
</ul>
</li>
<li><a href="#Agent-Types" title="Agent Types">Agent Types</a><ul>
<li><a href="#Physical-Agents" title="Physical Agents">Physical Agents</a></li>
<li><a href="#Software-Agents" title="Software Agents">Software Agents</a></li>
</ul>
</li>
<li><a href="#Abstract-Architecture" title="Abstract Architecture">Abstract Architecture</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Agent-Properties" data-id="Agent-Properties"><a class="anchor hidden-xs" href="#Agent-Properties" title="Agent-Properties"><span class="octicon octicon-link"></span></a><span>Agent Properties</span></h2><h3 id="Agent-Definitions" data-id="Agent-Definitions"><a class="anchor hidden-xs" href="#Agent-Definitions" title="Agent-Definitions"><span class="octicon octicon-link"></span></a><span>Agent Definitions</span></h3><blockquote>
<ul>
<li><span>Autonomous agents are computational systems that inhabit some </span><strong><span>complex dynamic environment</span></strong><span>, sense and </span><strong><span>act</span></strong><span> autonomously in this environment, and by doing so realize a set of </span><strong><span>goals or tasks</span></strong><span> for which they are designed.</span></li>
<li><span>An autonomous agent is a </span><strong><span>system situated within and a part of an environment that senses that environment and acts on it</span></strong><span>, over time, in pursuit of its </span><strong><span>own agenda</span></strong><span> and so as to affect what it senses in the future.</span></li>
</ul>
</blockquote><h3 id="Autonomy" data-id="Autonomy"><a class="anchor hidden-xs" href="#Autonomy" title="Autonomy"><span class="octicon octicon-link"></span></a><span>Autonomy</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>An agent is a computer system capable of </span><strong><span>autonomous</span></strong><span> action in some environment in order to meet its design objectives. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><p><span>Usually the environment is </span><strong><span>complex</span></strong><span> and </span><strong><span>dynamic</span></strong><span>, and agents should interact with it in real time.</span><br>
<u><span>Main property</span></u><span>: </span><strong><span>Autonomy</span></strong><span> capable of acting independently, exhibiting control over their </span><strong><span>internal state</span></strong><span>.</span></p><p><img src="https://i.imgur.com/msjmjkL.png" alt="" loading="lazy"></p><h3 id="Flexibility" data-id="Flexibility"><a class="anchor hidden-xs" href="#Flexibility" title="Flexibility"><span class="octicon octicon-link"></span></a><span>Flexibility</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>An intelligent agent is a computer system capable of </span><strong><span>flexible</span></strong><span> autonomous action in some environment. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><p><span>By flexible, we mean:</span></p><ul>
<li><span>Reactive (response capability).</span></li>
<li><span>Pro-active (taking initiative).</span></li>
<li><span>Social (interacting with others).</span></li>
</ul><h3 id="Reactivity" data-id="Reactivity"><a class="anchor hidden-xs" href="#Reactivity" title="Reactivity"><span class="octicon octicon-link"></span></a><span>Reactivity</span></h3><ul>
<li><span>A </span><strong><u><span>reactive system</span></u></strong><span> is one that maintains an ongoing interaction with its environment, and responds to changes that occur in it (in time for the response to be useful).</span></li>
<li><span>If a program’s environment is guaranteed to be fixed, the program need never worry about its own success or failure – program just executes blindly.</span>
<ul>
<li><span>Example of fixed environment: compiler.</span></li>
</ul>
</li>
<li><span>The real world is not like that: things change, </span><strong><span>information is incomplete</span></strong><span>. Many (most?) interesting environments are </span><strong><span>dynamic</span></strong><span>.</span></li>
<li><span>Software is hard to build for dynamic domains: program must take into account possibility of failure – </span><strong><span>ask itself whether it is worth executing!</span></strong></li>
</ul><h3 id="Proactivness" data-id="Proactivness"><a class="anchor hidden-xs" href="#Proactivness" title="Proactivness"><span class="octicon octicon-link"></span></a><span>Proactivness</span></h3><ul>
<li><u><strong><span>Pro-activeness</span></strong></u><span>: generating and attempting to achieve goals; not driven solely by events; </span><strong><span>taking the initiative</span></strong><span>.</span></li>
<li><span>Reacting to an environment is easy (stimulus → response rules), but we generally want agents to do things for us, hence </span><strong><span>goal directed behavior</span></strong><span>, </span><strong><span>recognizing opportunities.</span></strong></li>
</ul><h3 id="Social-Ability" data-id="Social-Ability"><a class="anchor hidden-xs" href="#Social-Ability" title="Social-Ability"><span class="octicon octicon-link"></span></a><span>Social Ability</span></h3><ul>
<li><strong><u><span>Social ability</span></u></strong><span> in agents is the ability to interact with other agents (and possibly humans) via some kind of </span><strong><span>agent-communication language</span></strong><span>, and perhaps cooperate with others.</span></li>
<li><span>The real world is a </span><strong><span>multi-agent</span></strong><span> environment: we cannot go around attempting to achieve goals without taking others into account.</span>
<ul>
<li><span>Some goals can only be achieved with the cooperation of others. Similarly for many computer environments: witness the Internet.</span></li>
</ul>
</li>
</ul><h3 id="Balancing-Reactive-and-Goal-Oriented-Behaviour" data-id="Balancing-Reactive-and-Goal-Oriented-Behaviour"><a class="anchor hidden-xs" href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing-Reactive-and-Goal-Oriented-Behaviour"><span class="octicon octicon-link"></span></a><span>Balancing Reactive and Goal-Oriented Behaviour</span></h3><p><span>These two considerations can be at odds with one another:</span></p><ul>
<li><span>We want our agents to be reactive, responding to changing conditions in an appropriate (timely) fashion.</span></li>
<li><span>We want our agents to systematically work towards longterm goals.</span></li>
</ul><blockquote style="border-left-color: rgb(255, 0, 0);">
<p><strong><span>Reactiveness vs. Deliberation balance</span></strong><br>
<span>Designing an agent that can balance reactiveness and deliberation (reason about long term goals) remains an openresearch problem. </span><span class="color" data-color="#ff0000"></span></p>
</blockquote><h3 id="Other" data-id="Other"><a class="anchor hidden-xs" href="#Other" title="Other"><span class="octicon octicon-link"></span></a><span>Other</span></h3><p><span>(Desireable, not mandatory)</span></p><ul>
<li><strong><span>Mobility</span></strong><span>: the ability of an agent to move around an electronic network.</span></li>
<li><strong><span>Veracity</span></strong><span>: an agent will not knowingly communicate false information</span></li>
<li><strong><span>Benevolence</span></strong><span>: agents do not have conflicting goals, and that every agent will therefore always try to do what is asked of it.</span></li>
<li><strong><span>Rationality</span></strong><span>: agent will act in order to achieve its goals, and will not act in such a way as to prevent its goals being achieved — at least insofar as its beliefs permit.</span></li>
<li><strong><span>Learning/Adaption</span></strong><span>: agents improve performance over time.</span></li>
</ul><hr><h2 id="Environment-Properties" data-id="Environment-Properties"><a class="anchor hidden-xs" href="#Environment-Properties" title="Environment-Properties"><span class="octicon octicon-link"></span></a><span>Environment Properties</span></h2><h3 id="Accessible-vs-Inaccessible" data-id="Accessible-vs-Inaccessible"><a class="anchor hidden-xs" href="#Accessible-vs-Inaccessible" title="Accessible-vs-Inaccessible"><span class="octicon octicon-link"></span></a><span>Accessible vs. Inaccessible</span></h3><ul>
<li><span>An </span><strong><u><span>accessible environment</span></u></strong><span> is one in which the agent can obtain complete, accurate, up-to-date information about the environment’s state (the environment is </span><strong><span>fully observable</span></strong><span>).</span></li>
<li><span>Most moderately complex environments (including, for example, the everyday physical world and the Internet) are </span><strong><u><span>inaccessible</span></u></strong><span> (or </span><strong><span>partially observable</span></strong><span>).</span></li>
<li><span>The more accessible an environment is, the simpler it is to build agents to operate in it.</span></li>
</ul><h3 id="Deterministic-vs-non-Deterministic" data-id="Deterministic-vs-non-Deterministic"><a class="anchor hidden-xs" href="#Deterministic-vs-non-Deterministic" title="Deterministic-vs-non-Deterministic"><span class="octicon octicon-link"></span></a><span>Deterministic vs. non-Deterministic</span></h3><ul>
<li><span>A </span><strong><u><span>deterministic environment</span></u></strong><span> is one in which any action has a single guaranteed effect — there is no uncertainty about the state that will result from performing an action.</span>
<ul>
<li><span>If the environment is deterministic except for the actions of other agents, then the environment can be defined as </span><strong><span>strategic</span></strong><span>.</span></li>
</ul>
</li>
<li><span>The physical world can to all intents and purposes be regarded as </span><strong><u><span>non-deterministic (or stochastic)</span></u></strong><span> Non-deterministic environments present greater problems for the agent designer.</span></li>
</ul><h3 id="Episodic-vs-non-Episodic" data-id="Episodic-vs-non-Episodic"><a class="anchor hidden-xs" href="#Episodic-vs-non-Episodic" title="Episodic-vs-non-Episodic"><span class="octicon octicon-link"></span></a><span>Episodic vs. non-Episodic</span></h3><ul>
<li><span>In an </span><strong><u><span>episodic environment</span></u></strong><span>, the performance of an agent is dependent on a number of discrete episodes, with </span><strong><span>no link</span></strong><span> between an agent’s performance in different scenarios.</span>
<ul>
<li><span>Episodic environments are simpler from the agent developer’s perspective because the agent can decide what action to perform based </span><strong><span>only on the current episode</span></strong><span> — it need not reason about the interactions between this and future episodes.</span></li>
</ul>
</li>
</ul><h3 id="Static-vs-Dynamic" data-id="Static-vs-Dynamic"><a class="anchor hidden-xs" href="#Static-vs-Dynamic" title="Static-vs-Dynamic"><span class="octicon octicon-link"></span></a><span>Static vs. Dynamic</span></h3><ul>
<li><span>A </span><strong><u><span>static environment</span></u></strong><span> is one that can be assumed to remain </span><strong><span>unchanged</span></strong><span> except by the performance of actions by the agent.</span></li>
<li><span>A </span><strong><u><span>dynamic environment</span></u></strong><span> is one that has </span><strong><span>other processes operating on it</span></strong><span>, and which hence changes in ways beyond the agent’s control. Other processes can interfere with the agent’s actions (as in concurrent systems theory).</span></li>
<li><span>The physical world is a highly dynamic environment.</span></li>
</ul><h3 id="Discrete-vs-Continuous" data-id="Discrete-vs-Continuous"><a class="anchor hidden-xs" href="#Discrete-vs-Continuous" title="Discrete-vs-Continuous"><span class="octicon octicon-link"></span></a><span>Discrete vs. Continuous</span></h3><ul>
<li><span>An </span><strong><u><span>environment is discrete</span></u></strong><span> if there are a </span><strong><span>fixed, finite number of actions and percepts</span></strong><span> in it.</span>
<ul>
<li><span>Discrete environments could </span><strong><span>in principle</span></strong><span> be handled by a kind of </span><strong><span>lookup table</span></strong><span>.</span></li>
</ul>
</li>
<li><span>Continuous environments have a certain level of mismatch with computer systems.</span></li>
<li><span>Russell and Norvig give a chess game as an example of a discrete environment, and taxi driving as an example of a continuous one.</span></li>
</ul><hr><h2 id="Agent-Types" data-id="Agent-Types"><a class="anchor hidden-xs" href="#Agent-Types" title="Agent-Types"><span class="octicon octicon-link"></span></a><span>Agent Types</span></h2><h3 id="Physical-Agents" data-id="Physical-Agents"><a class="anchor hidden-xs" href="#Physical-Agents" title="Physical-Agents"><span class="octicon octicon-link"></span></a><span>Physical Agents</span></h3><ul>
<li><span>Physical agents or embodied agents: Interact with real world (sensors, actuators connected to real world).</span></li>
<li><span>Problems of perception and action.</span></li>
<li><span>Best known example: Robots.</span></li>
</ul><h3 id="Software-Agents" data-id="Software-Agents"><a class="anchor hidden-xs" href="#Software-Agents" title="Software-Agents"><span class="octicon octicon-link"></span></a><span>Software Agents</span></h3><ul>
<li><span>Software agents’ environment is a virtual one: single machine, intranet, internet.</span>
<ul>
<li><span>Interact with other software agents, with software modules, services.</span></li>
<li><span>Interact with humans through human interfaces.</span></li>
</ul>
</li>
<li><span>Types of software agents:</span>
<ul>
<li><strong><span>Internet agents</span></strong><span> search and information extraction/management from Internet.</span></li>
<li><strong><span>Collaborative</span></strong><span> agents they coordinate with other agents to solve a common task.</span>
<ul>
<li><span>To solve problems too complex for a single agent.</span></li>
<li><span>To solve problems distributed in nature.</span></li>
<li><span>To interconnect already existing, heterogeneous systems (→ </span><strong><span>Agentification</span></strong><span>).</span></li>
</ul>
</li>
<li><strong><span>Interface agents</span></strong><span> they collaborate with a human user to solve a task, or to act on behalf of the user.</span></li>
<li><strong><span>Mobile SW agents</span></strong><span> they can move from one computer to another.</span></li>
</ul>
</li>
</ul><hr><h2 id="Abstract-Architecture" data-id="Abstract-Architecture"><a class="anchor hidden-xs" href="#Abstract-Architecture" title="Abstract-Architecture"><span class="octicon octicon-link"></span></a><span>Abstract Architecture</span></h2><ul>
<li><span>Internal architecture:</span>
<ul>
<li><span>Purely Reactive Agents (with no internal state).</span></li>
<li><span>Reactive Agents with internal state.</span></li>
<li><span>Delliberative Agents (goal-oriented behaviour).</span></li>
<li><span>Hybrid Agents (combine reactive and delliberative behaviour).</span></li>
</ul>
</li>
<li><em><span>Example</span></em><span>: A Multi-Agent System (Trading Agent Competition)!</span></li>
</ul><p><img src="https://i.imgur.com/ssergbT.png" alt="" loading="lazy"></p></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
<li><a href="#Agent-Types-and-Architectures" title="Agent Types and Architectures">Agent Types and Architectures</a><ul class="nav">
<li><a href="#Agent-Properties" title="Agent Properties">Agent Properties</a><ul class="nav">
<li><a href="#Agent-Definitions" title="Agent Definitions">Agent Definitions</a></li>
<li><a href="#Autonomy" title="Autonomy">Autonomy</a></li>
<li><a href="#Flexibility" title="Flexibility">Flexibility</a></li>
<li><a href="#Reactivity" title="Reactivity">Reactivity</a></li>
<li><a href="#Proactivness" title="Proactivness">Proactivness</a></li>
<li><a href="#Social-Ability" title="Social Ability">Social Ability</a></li>
<li><a href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing Reactive and Goal-Oriented Behaviour">Balancing Reactive and Goal-Oriented Behaviour</a></li>
<li><a href="#Other" title="Other">Other</a></li>
</ul>
</li>
<li><a href="#Environment-Properties" title="Environment Properties">Environment Properties</a><ul class="nav">
<li><a href="#Accessible-vs-Inaccessible" title="Accessible vs. Inaccessible">Accessible vs. Inaccessible</a></li>
<li><a href="#Deterministic-vs-non-Deterministic" title="Deterministic vs. non-Deterministic">Deterministic vs. non-Deterministic</a></li>
<li><a href="#Episodic-vs-non-Episodic" title="Episodic vs. non-Episodic">Episodic vs. non-Episodic</a></li>
<li><a href="#Static-vs-Dynamic" title="Static vs. Dynamic">Static vs. Dynamic</a></li>
<li><a href="#Discrete-vs-Continuous" title="Discrete vs. Continuous">Discrete vs. Continuous</a></li>
</ul>
</li>
<li><a href="#Agent-Types" title="Agent Types">Agent Types</a><ul class="nav">
<li><a href="#Physical-Agents" title="Physical Agents">Physical Agents</a></li>
<li><a href="#Software-Agents" title="Software Agents">Software Agents</a></li>
</ul>
</li>
<li><a href="#Abstract-Architecture" title="Abstract Architecture">Abstract Architecture</a></li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
            </ul>
        </div>
    </div>
    <div id="ui-toc-affix" class="ui-affix-toc ui-toc-dropdown unselectable hidden-print" data-spy="affix" style="top:17px;display:none;" null null>
        <div class="toc"><ul class="nav">
<li><a href="#Agent-Types-and-Architectures" title="Agent Types and Architectures">Agent Types and Architectures</a><ul class="nav">
<li><a href="#Agent-Properties" title="Agent Properties">Agent Properties</a><ul class="nav">
<li><a href="#Agent-Definitions" title="Agent Definitions">Agent Definitions</a></li>
<li><a href="#Autonomy" title="Autonomy">Autonomy</a></li>
<li><a href="#Flexibility" title="Flexibility">Flexibility</a></li>
<li><a href="#Reactivity" title="Reactivity">Reactivity</a></li>
<li><a href="#Proactivness" title="Proactivness">Proactivness</a></li>
<li><a href="#Social-Ability" title="Social Ability">Social Ability</a></li>
<li><a href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing Reactive and Goal-Oriented Behaviour">Balancing Reactive and Goal-Oriented Behaviour</a></li>
<li><a href="#Other" title="Other">Other</a></li>
</ul>
</li>
<li><a href="#Environment-Properties" title="Environment Properties">Environment Properties</a><ul class="nav">
<li><a href="#Accessible-vs-Inaccessible" title="Accessible vs. Inaccessible">Accessible vs. Inaccessible</a></li>
<li><a href="#Deterministic-vs-non-Deterministic" title="Deterministic vs. non-Deterministic">Deterministic vs. non-Deterministic</a></li>
<li><a href="#Episodic-vs-non-Episodic" title="Episodic vs. non-Episodic">Episodic vs. non-Episodic</a></li>
<li><a href="#Static-vs-Dynamic" title="Static vs. Dynamic">Static vs. Dynamic</a></li>
<li><a href="#Discrete-vs-Continuous" title="Discrete vs. Continuous">Discrete vs. Continuous</a></li>
</ul>
</li>
<li><a href="#Agent-Types" title="Agent Types">Agent Types</a><ul class="nav">
<li><a href="#Physical-Agents" title="Physical Agents">Physical Agents</a></li>
<li><a href="#Software-Agents" title="Software Agents">Software Agents</a></li>
</ul>
</li>
<li><a href="#Abstract-Architecture" title="Abstract Architecture">Abstract Architecture</a></li>
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
