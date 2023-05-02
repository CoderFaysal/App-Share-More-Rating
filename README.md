# Share App, More App, Rating App, Call Button, Url Button

## Share App

```
try {
                    Intent intent = new Intent(Intent.ACTION_SEND);
                    intent.setType("text/plain");
                    intent.putExtra(Intent.EXTRA_SUBJECT, "share app");
                    String shareMassage = "https://play.google.com/store/apps/details?id=com.coderfaysal.zakatcalculator";
                    intent.putExtra(Intent.EXTRA_TEXT, shareMassage);
                    startActivity(Intent.createChooser(intent, "Share by"));
                } catch (Exception e) {
                    Toast.makeText(MainActivity.this, "Error occurred", Toast.LENGTH_SHORT).show();
                }
```

## More App

```
try {
     startActivity(new Intent(Intent.ACTION_VIEW, Uri.parse("market://search?q=pub:Innovative Programmer")));
     } catch (android.content.ActivityNotFoundException anfe) {
     startActivity(new Intent(Intent.ACTION_VIEW, Uri.parse("https://play.google.com/store/apps/dev?id=5338546810958790262")));
     }
```

## Rating App

```
startActivity(new Intent(Intent.ACTION_VIEW, Uri.parse("https://play.google.com/store/apps/details?id=com.coderfaysal.zakatcalculator")));
```


## Url Button

```
startActivity(new Intent(Intent.ACTION_VIEW, Uri.parse("https://play.google.com/store/apps/details?id=com.coderfaysal.zakatcalculator")));
```


## Call Button

```
Intent intent = new Intent(Intent.ACTION_DIAL);
                intent.setData(Uri.parse("tel:+8801892837253"));
                startActivity(intent);
```


