# Pasar data por Intent Android

## Set

```java
Intent go = new Intent(FromActivity.this,ToActivity.class);
go.putExtra("key","value");
startActivity(go);
```

## Get

```java
String info = getIntent().getStringExtra("key");
```
