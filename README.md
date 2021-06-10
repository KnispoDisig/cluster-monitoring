### Конфигурация кластера Kubernetes с развертыванием категориальной абстрактной машины

- `camachine-dev` - содержатся основные файлы для пространств имен `prod` и `dev`, такие как деплоймент `camachine`, сервис для него, а также RBAC-объекты.
- `logging` - содержатся файлы, отвечающие за систему логгирования кластера с помощью `Fluentd` и `Elasticsearch` (пространство имен `kube-logging`).
- `monitoring` - содержатся файлы, отвечающие за систему мониторинга кластера (пространство имен `kube-monitoring`).

---

Также для настройки системы мониторинга кластера использовался следующий [helm-чарт](https://github.com/helm/charts/tree/master/stable/prometheus-operator). Команда:

```bash
helm install stable/prometheus-operator
```


<style>#mermaid-1621883399262{font-family:sans-serif;font-size:16px;fill:#333;}#mermaid-1621883399262 .error-icon{fill:#552222;}#mermaid-1621883399262 .error-text{fill:#552222;stroke:#552222;}#mermaid-1621883399262 .edge-thickness-normal{stroke-width:2px;}#mermaid-1621883399262 .edge-thickness-thick{stroke-width:3.5px;}#mermaid-1621883399262 .edge-pattern-solid{stroke-dasharray:0;}#mermaid-1621883399262 .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-1621883399262 .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-1621883399262 .marker{fill:#333333;}#mermaid-1621883399262 .marker.cross{stroke:#333333;}#mermaid-1621883399262 svg{font-family:sans-serif;font-size:16px;}#mermaid-1621883399262 .label{font-family:sans-serif;color:#333;}#mermaid-1621883399262 .label text{fill:#333;}#mermaid-1621883399262 .node rect,#mermaid-1621883399262 .node circle,#mermaid-1621883399262 .node ellipse,#mermaid-1621883399262 .node polygon,#mermaid-1621883399262 .node path{fill:#ECECFF;stroke:#9370DB;stroke-width:1px;}#mermaid-1621883399262 .node .label{text-align:center;}#mermaid-1621883399262 .node.clickable{cursor:pointer;}#mermaid-1621883399262 .arrowheadPath{fill:#333333;}#mermaid-1621883399262 .edgePath .path{stroke:#333333;stroke-width:1.5px;}#mermaid-1621883399262 .flowchart-link{stroke:#333333;fill:none;}#mermaid-1621883399262 .edgeLabel{background-color:#e8e8e8;text-align:center;}#mermaid-1621883399262 .edgeLabel rect{opacity:0.5;background-color:#e8e8e8;fill:#e8e8e8;}#mermaid-1621883399262 .cluster rect{fill:#ffffde;stroke:#aaaa33;stroke-width:1px;}#mermaid-1621883399262 .cluster text{fill:#333;}#mermaid-1621883399262 div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:sans-serif;font-size:12px;background:hsl(80,100%,96.2745098039%);border:1px solid #aaaa33;border-radius:2px;pointer-events:none;z-index:100;}#mermaid-1621883399262:root{--mermaid-font-family:sans-serif;}#mermaid-1621883399262:root{--mermaid-alt-font-family:sans-serif;}#mermaid-1621883399262 flowchart{fill:apa;}</style>
