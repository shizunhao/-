# -拾遗  补缺

#滚动条产生查询
# 控制台粘贴以下代码
function findScroller(element) {
    element.onscroll = function() { console.log(element)}

    Array.from(element.children).forEach(findScroller);
}

findScroller(document.body);
