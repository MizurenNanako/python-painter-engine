# Python Wrapper for *Painter Engine*

Possibly a Python Wrapper for [Painter Engine](https://github.com/matrixcascade/PainterEngine), if I have enough time to spend for.

According to Its [API](https://www.painterengine.com/manual.html), which written in Chinese and have no English translation, it seems to be an algorithm soup consists of following parts:

```mermaid
flowchart LR
    A[Painter Engine]
    A --> B[Core]
    A --> C[Kernel]
    subgraph Core
        direction LR
        B --> b1[pre-compile]
        B --> b2[log]
        B --> b3[allocator]
        B --> b4[memory pool]
        B --> b5[string]
        B --> b6[conversion]
        B --> b7[byte]
        B --> b8[math]
        B --> b9[IO layer]
        B --> ba[structure]
        B --> bb[geometry]
        B --> bc[graphics]
        B --> bd[font]
        B --> bf[signal processing]
        B --> bg[backpropagation]
        B --> bh[physics]
        B --> bi[cryptology]
        B --> bj[encoding]
        B --> bk[3D pipeline]
    end
    subgraph Kernel
        direction LR
        C --> c1[lexical analysis]
        C --> c2[painterscript]
        C --> c3[painterscript VM]
        C --> c4[Obj 3D static module loader]
        C --> c5[Live Framework]
        C --> c6[Live]
        C --> c7[particle system]
        C --> c8[MOTT]
        C --> c9[resource manager]
        C --> ca[frame synchronization]
        C --> cb[JSON]
        C --> cc[Object]
        C --> cd[Event]
        C --> ce[UI]
        C --> cf[UI framework]
        C --> cg[World]
    end
```

Most of the *Core* are reinvented wheels, ignoring [glib](https://github.com/GNOME/glib). However, compared to glib, this will take less time to wrap and will be a better practice.
