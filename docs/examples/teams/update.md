import 'package:appwrite/appwrite.dart';

// Init SDK
Client client = Client();
Teams teams = Teams(client);

client
    .setProject('5df5acd0d48c2') // Your project ID
;

Future result = teams.update(
    teamId: '[TEAM_ID]',
    name: '[NAME]',
);

result
  .then((response) {
    print(response);
  }).catchError((error) {
    print(error);
  });