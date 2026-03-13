// Fichier Service Worker minimum pour autoriser l'installation de la PWA
self.addEventListener('install', (e) => {
  self.skipWaiting();
});

self.addEventListener('activate', (e) => {
  return self.clients.claim();
});

self.addEventListener('fetch', (e) => {
  // Laisse le navigateur gérer les téléchargements normalement
  e.respondWith(fetch(e.request));
});