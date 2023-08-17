---
description: Bundler에 대하여.
layout:
  title:
    visible: false
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 📘 Bundler

## Parcel

```
특별한 설정 없이 바로 사용 가능한 빌드 도구.
```

{% tabs %}
{% tab title="참고 링크" %}
[https://github.com/ahastudio/til/tree/main/parcel](https://github.com/ahastudio/til/tree/main/parcel)

***

{% embed url="https://github.com/elwin013/parcel-reporter-static-files-copy" %}
ParcelJS v2 plugin to copy static files
{% endembed %}
{% endtab %}

{% tab title=".parcelrc 파일 작성" %}
{% code title=".parcelrc" lineNumbers="true" %}
```json
{
  "extends": ["@parcel/config-default"],
  "reporters": ["...", "parcel-reporter-static-files-copy"]
}
```
{% endcode %}
{% endtab %}
{% endtabs %}
