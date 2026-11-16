BUMPER REMOVER
- Select FRONT, REAR, or FRONT + REAR for one car or all cars.
- Single-car operation also requests the car ID.
Method: decode typeToInstall; slot 3 = front and slot 4 = rear. The selected slot(s) are set to -1. Slots 1 and 2 were already -1 in the inspected garage, so changing them did not remove the visible bumpers.
Login to target account first in Mini App.

Dashboard prompts offer Front bumper, Rear bumper, and Front + rear bumpers for both single-car and all-car removal.
All-car removal preserves each car's existing generated ID, does not rewrite unrelated car vectors, paces saves, checks the API result code, and re-fetches the garage to verify the installed-part values.
