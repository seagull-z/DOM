window.dom = {
    find(node, score) {
        return (score || document).querySelectorAll(node)
    },
    // style(node, name, value) {
    //   debugger
    //   if (arguments.length === 3) {
    //     node.style[name] = value
    //   } else if (arguments.length === 2) {
    //     if (typeof name === 'string') {
    //       return node.style[name]
    //     } else if (name instanceof Object) {
    //       for (let key in name) {
    //         node.style[key] = name[key]
    //       }
    //     }
    //   }
    // }
    style(node, name, value) {
        if (arguments.length === 3) {
            // dom.style(div,'color','red')
            node.style[name] = value
        } else if (arguments.length === 2) {
            if (typeof name === 'string') {
                // dom.style(div,'color')
                return node.style[name]
            } else if (name instanceof Object) {
                // dom.style(div,'color:red')
                for (let key in name) {
                    node.style[key] = name[key]
                }
            }
        }
    },
    each(node, fn) {
        for (let i = 0; i < node.length; i++) {
            fn.call(null, node[i])
        }
    }
}