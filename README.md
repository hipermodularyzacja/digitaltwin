# digitaltwin
reprezentacja cyfrowego blizniaka w formacie języków: kotlin, nodejs


```kotlin

class Network(val name: String, val nodes: List<Node>) {
    fun addNode(node: Node) {
        nodes += node
    }

    fun removeNode(node: Node) {
        nodes -= node
    }
    
    fun ping(node: Node) {
        // logic for pinging another node
    }

}

class Node(val modules: List<Module>) {

    
    fun addModule(module: Module) {
        modules += module
    }

    fun removeModule(module: Module) {
        modules -= module
    }
    
    fun ping(module: Module) {
        // logic for pinging another module
    }
}


class Module(val context: String, val contents: List<Content>) {
    
}

class Content(val content: String) {
        
    fun addContent(content: Content) {
        contents += content
    }

    fun removeContent(content: Content) {
        contents -= content
    }
}

```


przykład w oparciu o system regałów, skrzynek, zawartości:

Network: środowisko, pokój, samochód
Node: regał, półka, szerokość, wysokość
Module: Skrzynka, 
Zawartość: Context: HDMI, USB, RPI (kable, zasilacze, płyty, obudowy)
