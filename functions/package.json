const functions = require('firebase-functions');
const admin = require('firebase-admin');
admin.initializeApp();

exports.addHealthData = functions.https.onRequest(async (req, res) => {
  if (req.method !== 'POST') return res.status(405).send('Method Not Allowed');
  // Optionally, verify Firebase Auth token here

  const { userId, heartRate, timestamp } = req.body;
  await admin.firestore().collection('healthData').add({ userId, heartRate, timestamp });
  res.status(200).send({ success: true });
});
