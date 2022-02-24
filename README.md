# clean-data

`
const data = {
    a: 'foo',
    b: 'bar',
    c: null,
    d: undefined,
    e: 0,
    f: {
        a: 'fuz',
        b: null,
        c: {
            a: 'biz',
            b: 'buz',
            c: '123',
            d: [{
                    a: 'foo',
                    b: 'bar',
                    c: null,
                    d: undefined,
                    e: 0,
                    f: false,
                    g: 12,
                    h: '13',
                    i: {},
                    j: [],
                    k: [
                        []
                    ]
                },
                {
                    a: 'foo',
                    b: 'bar',
                    c: null,
                    d: undefined,
                    e: 0
                },
                {
                    a: 'foo',
                    b: 'bar',
                    c: null,
                    d: undefined,
                    e: 0,
                    f: '-7',
                    g: '3.14159265358979323'
                }
            ]
        }
    },
    g: 123,
    h: '456',
    i: false,
    j: {},
    k: [],
    l: [
        []
    ],
    m: '3.14159265358979323'
};
`

Challenge, refactor this cleanse function so it accomplishes the following criteria
data is not mutated
all `null` and `undefined` values are omitted from the returned data tree
all stringified numbers are converted to numbers. Example, '123' becomes 123.
