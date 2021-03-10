# Pasar data por Intent Android

## Set

```java
Intent go = new Intent(FromActivity.this,ToActivity.class);
go.putExtra("key","value");
startActivity(go);

// With parcelable
Intent intent = new Intent(getBaseContext(), NextActivity.class);
Foo foo = new Foo();
intent.putExtra("foo ", foo);
startActivity(intent);
```

## Get

```java
String info = getIntent().getStringExtra("key");

// With ParceLable
Foo foo = getIntent().getExtras().getParcelable("foo");
```

