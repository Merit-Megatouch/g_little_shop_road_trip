# ROAD TRIP (g_little_shop_road_trip)

Status: scaffolded 2026-10-07. Facts: [notes/scaffold.md](notes/scaffold.md).

## Checklist
- [ ] Window size in game.conf matches the largest PNG (notes/scaffold.md)
- [ ] Every symbol in notes/unresolved.txt has a stand-in in src/host/loader_services.cpp
      (`make analyze GAME=g_little_shop_road_trip` until it reports 0)
- [ ] First run: `make run GAME=g_little_shop_road_trip DEBUG=shots` — crash trace + screenshots in notes/shots
- [ ] Paths: `make run GAME=g_little_shop_road_trip DEBUG=files`; engine trace: `mkdir -p data/var/merit/debug/files && touch data/var/merit/debug/files/resource_locator`
- [ ] Reference code: `make decompile GAME=g_little_shop_road_trip`
- [ ] Translations + help text appear (gamedata/translations/g_little_shop_road_trip.utf8)
- [ ] Sound and music play (`DEBUG=sound`)
- [ ] A full game plays through (`DEBUG=profile` to catch stalls and old-malloc bugs)

## Log
<!-- dated notes: what broke, what fixed it -->
