import 'package:appwrite/appwrite.dart';

// Init SDK
Client client = Client();
Teams teams = Teams(client);

client
    .setProject('5df5acd0d48c2') // Your project ID
;

Future result = teams.list(
);

result
  .then((response) {
    print(response);
  }).catchError((error) {
    print(error);
  });