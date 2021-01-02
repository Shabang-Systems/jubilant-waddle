# jubilant-waddle
A backtracing algo for Nueva

Let's do this like an algos problem, why the heck not?

`waddle.in`

The first line contains number of blocks per week `B`, number of classes `C`, number of students `N`, number of teachers `T` and finally total school semester duration `S`

The next `B` lines `Bi` has three numbers `B_ia`, `B_ib`, `B_id`, representing the start and end hours inclusive (`1 1` means it takes the whole of 1AM, we'll do this by hours) by which each block exists. `1 <= B_i <= 24`. For simplicity let's say `B_ia < B_ib`, so no cross-day blocks. At the moment, a block is a block — so no block aparteid at the moment for simplicity (i.e. a block starting at 11 is the same as a block starting at 21. A block on Tuesday is the same as a block on Friday). Because of the fact that there is no block discrimination, `B_id` — the day of week on which the block exists is just metadata. `1 <= B_id <= 5` Let's also assume that no two blocks overlap with each other. (That is, if two blocks occur at the same time, they are on different days.)

Then, the next `C` lines `Ci` contains two numbers `Ci_{total}` and `Ci_{week}`, representing the total runtime of the class and the runtime of the class per week. Let's call these numbers `<1e3`. "Course numbers" are also devised this way, where course `i` is the `i`th course (so... 1 indexed to make @Exr0n happy.)

After that, the next `N` lines `Ni` contains numbers `Ni_{required}` and `Ni_{elective}`, followed by `Ni_{required}` number of required courses `Ni_rc` and `Ni_ec` number of elective courses with `1<=Ni_ec<=C`. Notably, the count of `Ni_ec` may be bigger than `Ni_{elective}`: students could sign up for more courses than they could take. For simplicity's sake, all students are eligible to take all classes.



