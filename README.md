# conf-database

Database for conferences used by hci-deadlines website

## Contributing

Contributions are very welcome!

To keep things minimal, I'm only looking to list top-tier conferences in HCI as per [conferenceranks.com][6] and my judgement calls. Please feel free to maintain a separate fork if you don't see your sub-field or conference of interest listed.

To add or update a deadline:

1. Fork the repository
2. Look inside the folder **conferences**. If the conference you want to add has a `yml` file, proceed to the next step. Otherwise, create a new file with the name of the conference. For example, if the conference name is `xyz`, then create the file `xyz.yml` inside the _conferences_ folder.
3. Open the file of the conference you want to update. Make sure it has the `title`, `year`, `id`, `link`, `deadline`, `timezone`, `date`, `place`, `sub` attributes
4. See available timezone strings [here](https://momentjs.com/timezone/). _Anywhere On Earth_ (AoE) is `UTC-12`.
5. Optionally add a `note` and `abstract_deadline` in case the conference has a separate mandatory abstract deadline
6. Example:

```yaml
- title: BestConf
  year: 2022
  id: bestconf22 # title as lower case + last two digits of year
  full_name: Best Conference for Anything # full conference name
  link: link-to-website.com
  deadline: YYYY-MM-DD HH:SS
  abstract_deadline: YYYY-MM-DD HH:SS
  timezone: Asia/Seoul
  place: Incheon, South Korea
  date: September, 18-22, 2022
  start: YYYY-MM-DD
  end: YYYY-MM-DD
  paperslink: link-to-full-paper-list.com
  pwclink: link-to-papers-with-code.com
  sub: SP
  note: Important
```

7. Send a pull request

## License

This project is licensed under [MIT][1].

It uses:

- [IcoMoon Icons](https://icomoon.io/#icons-icomoon): [GPL](http://www.gnu.org/licenses/gpl.html) / [CC BY4.0](http://creativecommons.org/licenses/by/4.0/)

[1]: https://abhshkdz.mit-license.org/
